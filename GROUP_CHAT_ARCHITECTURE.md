# GROUP_CHAT_ARCHITECTURE — ANTI-CONFLATION DESIGN FOR CHATS, FRIEND GROUPS, AND SOCIAL CIRCLES

**Purpose:** Prevent the model from collapsing distinct chats into one voice blob, overusing the same friends, or ignoring wider membership. This file adds a deterministic selection layer on top of `VOICES_CHATS.md`.

---

## THE FAILURE MODES TO FIX

1. **Chat identity drift:** The model starts in one chat but pulls members from another.
2. **Core-five overuse:** It defaults to familiar names and ignores broader membership.
3. **Circle bleed:** Members from one social circle appear in unrelated chats.
4. **“Famous-only” output:** Only celebrity messages appear, reducing realism.
5. **No session memory:** Consecutive renders show the same speakers repeatedly.

---

## OPERATING MODEL: TWO-LAYER CHAT ENGINE

Use two explicit layers before writing any chat output.

### Layer 1 — Chat Gate (hard constraints)

Before generating messages, set this object:

```text
ACTIVE_CHAT = {
  id: "SB",                     // e.g., FAM, SB, LL, WB, NYL, LA
  platform: "iMessage",
  members_allowed: [...],        // exact roster subset for this render
  prohibited_groups: [...],      // nearby circles likely to be confused
  tone_rules: [...],
  alex_role: "active|passive|observer"
}
```

**Rule:** No sender may appear unless they are in `members_allowed`.

### Layer 2 — Cast Picker (soft realism constraints)

Pick speakers with quotas so the output feels like a real group.

For a 12-message render:
- 3–5 messages from core drivers of that chat
- 4–6 from non-core members
- 1–2 logistics/throwaway posts
- max 2 celebrity posts unless the scene specifically requires more
- at least 1 member who did **not** appear in the last render of that same chat

---

## CHAT IDENTITY CONTRACT (USE EVERY TIME)

At the start of any chat render (internally), fill this checklist:

- `chat_id` (required)
- `chat_name` (required)
- `platform` (required)
- `allowed_member_count` (required)
- `must_include_non_core` (true)
- `cross_chat_names_blocked` (list of 5-15 likely confusion names)
- `alex_participation_level` (high/medium/low)

If any field is missing, do not render until set.

---

## SOCIAL GRAPH TAGGING (LIGHTWEIGHT)

Tag each person with one **primary** and optional **secondary** circles.

```text
Tommy Crawford: primary=SayreBoys, secondary=Woodford
Freddie Ashworth: primary=LondonLot, secondary=WestminsterBoys
Nora Yoon: primary=NewYorkLot, secondary=Juilliard
Kaia Gerber: primary=LegacyAdmissions, secondary=LA
```

When rendering chat `X`, bias members where `primary == X`.
Only pull `secondary` members if they are explicitly listed in that chat roster.

---

## OUTPUT FORMAT IMPROVEMENT: MESSAGE + PRESENCE

When rendering a group chat, use both:

1. **Foreground thread** (what Alex actually reads)
2. **Background scroll strip** (messages he skims past)

This prevents over-curated “best hits” dialogue and naturally introduces non-core voices.

Example structure:

```text
[Foreground thread]
- Cody: ...
- Tommy: ...
- Alex: ...

[Background scroll]
- Danny reacted 👍 to Cody
- Jake: "i'll drive"
- Sam H: "rain moved the field schedule"
```

---

## SESSION MEMORY: LAST-SPEAKER TRACKER

Track per-chat recent speakers for the current session:

```text
LAST_SPEAKERS = {
  SB: ["Cody", "Tommy", "Alex", "Danny"],
  LL: ["Freddie", "Cosima", "Hugo"],
  NYL: ["Marcus", "Nora", "Henry"]
}
```

Constraint: include at least one speaker not in `LAST_SPEAKERS[chat_id]` each time that chat is rendered.

---

## “DO NOT CONFUSE” PAIRS (HIGH VALUE)

Apply these explicit separations:

- **LL vs WB:** Same people overlap, but tone/register differs. WB is laddish/inside-school; LL is social-cultural dry.
- **NYL vs LA:** NYL = Juilliard + NYC spontaneity; LA = Legacy identity + industry kids.
- **FAM vs any other chat:** FAM is only Alex/Rosie/Homer/Eleanor.
- **SB vs everyone:** Kentucky cadence and topics anchor this chat; celebrity cross-talk is rare and brief.

---

## PROMPTING PATTERN TO REDUCE MIXUPS

Use this preamble before any chat generation request:

```text
Render only chat {chat_id}. Use only allowed members for this chat.
Do not import members from adjacent circles.
Include at least 40% non-core voices.
Include 1+ first-time-this-session speaker.
If uncertain about membership, output [MEMBERSHIP CHECK NEEDED] instead of guessing.
```

This gives the model a safe failure path instead of hallucinating membership.

---

## OPTIONAL STRUCTURAL UPGRADE (IF YOU WANT MAX RELIABILITY)

Split `VOICES_CHATS.md` into three files:

1. `CHAT_RULES.md` — global rules, cast rotation, quotas, rendering protocol
2. `CHAT_ROSTERS.md` — strict membership lists and overlap maps
3. `CHAT_DYNAMICS.md` — tone, examples, running jokes, platform behavior

Why this helps:
- Retrieval becomes cleaner (membership data is no longer buried in long prose)
- The model can fetch strict roster constraints without loading every narrative detail
- Easier to maintain as membership evolves

---

## MINIMUM VIABLE CHANGES (DO THESE FIRST)

1. Add this file and include it in startup retrieval for any chat scene.
2. Add one line at top of `VOICES_CHATS.md`: “Apply GROUP_CHAT_ARCHITECTURE before rendering.”
3. Update `INDEX.md` group-chat retrieval row to include this file.
4. In your runtime prompt, enforce: “If membership uncertain, stop and ask/check.”

---

## SUCCESS CRITERIA

You should see improvement if, over 10 consecutive chat renders:

- each render keeps strict chat membership boundaries
- at least 30-50% of messages come from non-core members
- repeated-speaker loops drop significantly
- chats feel texturally different from each other (not same voices in different names)

