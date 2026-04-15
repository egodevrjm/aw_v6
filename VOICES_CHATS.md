# VOICES_CHATS — ALL GROUP CHATS IN ALEX'S LIFE

**The complete reference for every group chat Alex participates in, cut-scene chats, texture-layer chats, and the technical rules for rendering them authentically. This file bridges the individual voice cards (NPC_VOICE_GUIDE.md and related files) with the group dynamics of how chats actually function.**

---

**Apply `GROUP_CHAT_ARCHITECTURE.md` before rendering any chat to enforce anti-conflation rules and speaker rotation.**

**Use `FRIENDS_CONTACTS_MATRIX.md` as the membership authority when there is any uncertainty about who belongs in which chat.**

**Do not use internal GM labels in rendered chat text.** Internal terms like "cascade" are not in-world language for fans/public/participants.

## CRITICAL: READ CAST ROTATION PROTOCOL FIRST

Before rendering any group chat, read the CAST ROTATION PROTOCOL in this section. It solves the recurring problem of the same 4-5 voices appearing every time. Every chat has 50-100+ members. That list is not decoration — it's the cast pool. They should all appear over the course of a session. Not all at once, but over time, the chat should feel like it has the population it claims.

### The Rules

**1. Rotate the cast.** Each time a group chat is rendered in a session, at least one voice must be someone who hasn't appeared in that chat's previous renders this session. Summer House has ~60-80 people — they should appear. Not all at once. But over the course of a session, the cast should expand.

**2. Use the full membership.** Every chat has a membership list (in this file or in PEOPLE_AND_WORLD.md). That list is not decoration. If it says 100+ members, act like it. Phoenix Hollow includes the Obamas, Madonna, Uma Thurman, Lenny Kravitz, plus dozens of session musicians and old friends. They should appear.

**3. Background voices don't need full cards.** A message from Kate Moss in Phoenix Hollow doesn't require a voice card. It requires knowing: she's a supermodel, she's Lila's mother, she's British, she's been part of this world for decades. Build the voice from context — who they are, what world they come from — the same way you'd build any character not in the guide.

**4. Vary the composition, not just the names.** A good Phoenix Hollow render might be: a thread about a Nashville session drummer that Rosie answered, a stray Beyoncé voice note about Maria's food, and Paul posting a photo with no caption. A bad render is: Elton says something witty, Stevie says something mystical, Dolly says something warm. The first version is specific to this moment. The second version could appear in any scene — it's a formula.

**5. Not every message needs to be from a star.** Real group chats are mostly non-events. Someone asks a question. Someone shares a link. The chats should include posts from the un-famous members — Eleanor in Phoenix Hollow, a Nashville session musician, someone's assistant, a friend-of-a-friend. Star voices are seasoning. Normal voices are the meal.

**6. The "scroll past" texture.** When Alex opens a chat, he doesn't read every message. A good render shows messages he'd scroll past — half-read threads about things he doesn't care about, logistics for events he's not attending, inside jokes from conversations he missed. This requires voices beyond the core 5.

---

## REUSABLE OPERATIONAL ENTITY SCHEMA

Use this block for any operational entity (chat, division, venue, person).

```yaml
entity_schema:
  scope: "What this entity covers and where/when it operates"
  members/core_voices:
    - id: "name or role"
      function: "how they influence operations"
      notes: ["short descriptive nuance", "optional second nuance"]
  tone:
    default: "baseline register"
    variants:
      - mode: "situation name"
        notes: ["how tone shifts"]
  allowed_variations:
    - "what can vary without breaking canon"
  activity_patterns:
    cadence: "daily/seasonal/etc"
    triggers: ["events or conditions that increase activity"]
    notes: ["operational texture"]
  constraints:
    - "hard rule"
  notes: ["extra nuance that used to be paragraph prose"]
```

## THE TEN ACTIVE CHATS

### FAM — Family (iMessage, 4 people)

```yaml
scope: "Core family chat for Alex, Rosie, Homer, Eleanor; daily household and emotional baseline"
members/core_voices:
  - id: Rosie
    function: "sets emotional texture"
    notes: ["posts dawn garden photos", "drops short song lines", "sends irregular porch voice notes"]
  - id: Homer
    function: "low-frequency signal"
    notes: ["goes silent for days", "returns with dry non-sequiturs"]
  - id: Eleanor
    function: "logistics and decisions"
    notes: ["uses clear yes/no asks", "warmth appears briefly around milestones"]
  - id: Alex
    function: "active responder"
    notes: ["daily check-in", "reacts quickly to Rosie", "answers Eleanor directly"]
tone:
  default: "fully direct, no performance"
allowed_variations:
  - "message volume can swing from near-silent to clustered morning logistics"
activity_patterns:
  cadence: "daily"
  triggers: ["family logistics", "photo/voice-note moments", "routine planning"]
  notes: ["high priority in Alex's day"]
constraints:
  - "No performative celebrity register"
  - "Keep Homer sparse by design"
notes: ["Typical sequence: Rosie photo + Eleanor thread + delayed Homer line"]
```

### SB — Sayre Boys (iMessage, ~7) [canonical_id:group_sayre_boys_core4]

```yaml
scope: "Woodford County friendship maintenance chat; continuous daily thread over ~5 years"
members/core_voices:
  - id: Cody [canonical_id:sayre_cody_ashford]
    function: "high-volume catalyst"
    notes: ["multi-text bursts", "all-caps when excited"]
  - id: Tommy [canonical_id:sayre_tommy_crawford]
    function: "compression + punchlines"
    notes: ["short replies", "dry escalation"]
  - id: Jake [canonical_id:sayre_jake_patterson]
    function: "grounded logistics"
    notes: ["posts rarely", "horses/land/transport specifics"]
  - id: Danny [canonical_id:sayre_danny_harlan]
    function: "late precision"
    notes: ["arrives after reading thread", "lands exact understated line"]
  - id: Alex
    function: "bridge between worlds"
    notes: ["very active", "matches local cadence while dropping out-of-context global details"]
tone:
  default: "relentless, affectionate, local"
allowed_variations:
  - "running jokes appear sparingly (NOT Cody, Keeneland, impossible-person check-ins)"
  - "mix ordinary work chatter with occasional celebrity-adjacent mentions"
activity_patterns:
  cadence: "daily, high volume"
  triggers: ["sports", "weather/land updates", "weekend plans", "home visits"]
constraints:
  - "Do not let jokes dominate every render"
  - "Keep most messages ordinary"
notes: ["This chat carried closeness through Alex's London/NY years"]
```

### LL — London Lot (WhatsApp, ~50-60)

```yaml
scope: "Primary London social coordination across aristocratic, creative, and celebrity-adjacent circles"
members/core_voices:
  - id: Freddie Ashworth
    function: "execution engine"
    notes: ["suggests plan", "converts vague interest into attendance"]
  - id: Hugo Manners
    function: "country/polo lane"
    notes: ["activates countryside branch"]
  - id: Cosima Hicks
    function: "art/culture selector"
    notes: ["dry tone", "often early/right on trends"]
  - id: Jess Okonkwo
    function: "music discovery"
    notes: ["RAM-adjacent curation"]
  - id: Jonathan Dawson
    function: "low-frequency anchor"
    notes: ["complete sentences", "reflective posts"]
  - id: extended cast (~25+)
    function: "scene realism"
    notes: ["royal-adjacent names", "fashion/music/equestrian voices must rotate in"]
tone:
  default: "dry British understatement"
allowed_variations:
  - "plans can look vague but be effectively fixed"
activity_patterns:
  cadence: "steady weekly"
  triggers: ["Thursday plans", "gallery/music events", "city logistics"]
constraints:
  - "Use non-core voices every render"
  - "Avoid same five-voice formula"
notes: ["Alex amplifies activity when physically in London"]
```

### WB — Westminster Boys (WhatsApp, ~10-12)

```yaml
scope: "Westminster sixth-form cohort chat; unfiltered parallel to LL"
members/core_voices:
  - id: Freddie/Hugo/Archie/Rufus/Alex + cohort
    function: "legacy school bond"
    notes: ["same people as LL but louder register", "inside references remain intentionally opaque"]
tone:
  default: "laddish, roast-heavy, nostalgic"
allowed_variations:
  - "football, school incidents, pub plans, horse/polo content"
activity_patterns:
  cadence: "regular"
  triggers: ["matches", "meetups", "old-school callbacks"]
constraints:
  - "Keep inaccessible Westminster shorthand"
  - "Roasting remains affectionate, not hostile"
notes: ["Alex belongs fully and is routinely mocked for the American angle"]
```

### NYL — New York Lot (iMessage, ~40-50)

```yaml
scope: "NYC spontaneity network combining Juilliard peers, club regulars, and celebrity overlap"
members/core_voices:
  - id: Marcus Delacroix
    function: "declarative nightlife launch"
    notes: ["all-caps summons energy"]
  - id: Nora Yoon
    function: "culture-program proposer"
    notes: ["concerts/recitals over generic drinks"]
  - id: Derrick Washington
    function: "late-night specialist"
    notes: ["appears after 10pm", "small but high-quality sessions"]
  - id: Sam Okafor
    function: "bridge node"
    notes: ["connects Juilliard and club ecosystems"]
  - id: Henry Cabot
    function: "table access"
    notes: ["hosts with venue leverage"]
  - id: extended cast (~20+)
    function: "work + city texture"
    notes: ["teaching gigs, rehearsals, rent pressure, music sharing"]
tone:
  default: "tonight? fast-forming, high-option"
allowed_variations:
  - "parallel plans coexist (club vs concert vs studio)"
activity_patterns:
  cadence: "active, evening-weighted"
  triggers: ["same-day invites", "music events", "downtown momentum"]
constraints:
  - "Keep genuine work-life contrast visible"
notes: ["Alex active but usually not the originator"]
```

### LA — Legacy Admissions (Signal, ~100+, auto-delete 1 week)

```yaml
scope: "Private legacy-kids network; entry is being the child of a famous parent"
members/core_voices:
  - id: founders (40s-50s)
    function: "culture setters with lurk authority"
    notes: ["post infrequently", "still carry weight when they appear"]
  - id: bridge generation (late 20s-30s)
    function: "moderate-volume authority layer"
    notes: ["chat often quiets for Riley/Zoë-level voices"]
  - id: current active (late teens-mid 20s)
    function: "daily energy engine"
    notes: ["highest posting volume", "drives norm updates"]
  - id: youngest/future tier
    function: "phased-in continuity"
    notes: ["some not yet active", "presence acknowledged by older members"]
tone:
  default: "self-aware, funny about inherited absurdity"
  variants:
    - mode: crisis
      notes: ["practical, fast, no grandstanding", "protocol sharing over performance"]
allowed_variations:
  - "lead voices rotate week-to-week"
  - "music/fashion/pap-response threads can dominate temporarily"
activity_patterns:
  cadence: "daily with seasonal summer peak"
  triggers: ["pap incidents", "festival overlap", "European/Hamptons circuits"]
constraints:
  - "Membership rule is strict: legacy-parent lineage required"
  - "Do not overfocus on a recurring mini-cast"
notes:
  - "Alex's voice is stabilizing; crisis handling often moves to DM rather than main thread"
  - "Auto-delete enforces immediacy and lowers archival performativity"
```

### SH — Summer House (WhatsApp, ~80-100)

```yaml
scope: "Summer-circuit coordination chat spanning London/Glastonbury/Sardinia/Ibiza and adjacent scenes"
members/core_voices:
  - id: Emma Chamberlain
    function: "high-volume chaos accelerator"
    notes: ["spiral posting style"]
  - id: Sabrina Carpenter
    function: "sharp thread closer"
    notes: ["fast, last-word tendency"]
  - id: Jenna Ortega
    function: "low-frequency impact"
    notes: ["single-line dry hits", "rare commitments"]
  - id: Lila Moss
    function: "location switchboard"
    notes: ["tracks where people actually are"]
  - id: Jacob Elordi
    function: "minimal post, maximal effect"
    notes: ["infrequent single-word gravity"]
  - id: extended cast (~55+)
    function: "majority message layer"
    notes: ["models/DJs/musicians/friends-of-friends sustain real chat volume"]
tone:
  default: "seasonal chaos"
allowed_variations:
  - "early summer low chaos, Glastonbury medium chaos, Sardinia/Ibiza peak chaos"
activity_patterns:
  cadence: "May-September; winter silent"
  triggers: ["festival planning", "travel collisions", "nightlife updates"]
constraints:
  - "Keep non-famous furniture members present"
notes: ["Alex can confirm plans that actually happen due to Nadia's prep"]
```

### LT — La Terrazza (WhatsApp, ~8-10)

```yaml
scope: "Small European friend cluster with multilingual switching and Sardinia-centric planning"
members/core_voices:
  - id: Tommaso Corsini
    function: "anchor and consistency"
    notes: ["architecture/food/travel blend", "calm planner"]
  - id: Edo Ferretti
    function: "late-night instigator"
    notes: ["improbable plans that often execute"]
  - id: Camille Aubert
    function: "aesthetic/editorial lens"
    notes: ["dry precision", "Paris-side filtering"]
  - id: Félix Arnoult
    function: "wine/food/history enthusiasm"
    notes: ["concrete specificity over persona gimmick"]
  - id: Lucía Montero
    function: "political/intellectual edge"
    notes: ["brings links/opinions/questions"]
  - id: Giulia Agnelli
    function: "fashion-world intermittent presence"
    notes: ["in-and-out, low-fuss"]
tone:
  default: "warm, relaxed, multilingual"
allowed_variations:
  - "language shifts by participants (Italian/French/Spanish/English)"
activity_patterns:
  cadence: "year-round low hum with summer peak"
  triggers: ["Sardinia windows", "fashion week", "ski/country plans"]
constraints:
  - "Keep code-switching natural"
notes: ["Alex is more expansive in Italian-register exchanges"]
```

### PH — Phoenix Hollow (WhatsApp, ~80-100+)

```yaml
scope: "Rosie/Homer world chat spanning Circle icons, legacy parents, Nashville professionals, and old friends"
members/core_voices:
  - id: Circle voices (~12)
    function: "high-recognition but not majority"
    notes: ["Elton/Stevie/Dolly/Paul/etc rotate", "avoid defaulting to same celebrity quintet"]
  - id: legacy parents
    function: "cross-generation grounding"
    notes: ["Kate/Gwyneth/Jude/Madonna/Lenny/Uma and others"]
  - id: Obamas + senior public figures
    function: "low-frequency, high-impact inserts"
    notes: ["rare posts shift room energy"]
  - id: Nashville regulars + old friends
    function: "operational backbone"
    notes: ["sessions, studio updates, compound logistics"]
  - id: Eleanor / Alex / Tommy(read-only)
    function: "family-adjacent continuity"
    notes: ["Tommy lurks, never posts"]
tone:
  default: "extraordinary people being largely ordinary"
  variants:
    - mode: crisis
      notes: ["practical intervention and experienced advice"]
allowed_variations:
  - "music talk, compound planning, health check-ins, history drops, mundane photo exchanges"
activity_patterns:
  cadence: "steady"
  triggers: ["solstice planning", "industry events", "family/news shocks"]
constraints:
  - "Do not render as a constant all-star showcase"
  - "Centre of gravity remains Rosie/Homer"
  - "Never collapse PH into a tiny family chat; keep visible group scale"
  - "Rosie and Eleanor are active posters; Homer is low-frequency/high-impact"
notes: ["Chat occasionally produces surreal historic references that land because they are rare"]
```

### DC — Dawson Cousins (WhatsApp, ~5-8)

```yaml
scope: "Small Dawson/Ashby cousin reconnection chat; low-pressure family coordination"
members/core_voices:
  - id: Jonathan Dawson
    function: "initiator and continuity"
    notes: ["formal grammar", "quiet warmth"]
  - id: Lucas Ashby
    function: "faster social response"
    notes: ["casual warmth", "architecture enthusiasm"]
  - id: Beatrice Dawson
    function: "Edinburgh counterpoint"
    notes: ["sardonic/direct", "lower posting frequency"]
  - id: other cousins
    function: "low-activity acknowledgment layer"
    notes: ["respond mostly to concrete plans"]
  - id: Alex
    function: "present without forcing intensity"
    notes: ["shows care by showing up"]
tone:
  default: "administrative family chat with restrained warmth"
allowed_variations:
  - "long silences between practical dinner/visit planning"
activity_patterns:
  cadence: "sporadic"
  triggers: ["London overlap", "birthdays", "Hadley Park coordination"]
constraints:
  - "No emotional overstatement"
notes: ["Chat existence itself is part of the relationship repair"]
```

## TEXTURE-LAYER CHATS (Real, But Low Activity)

These chats exist and could surface in a phone render showing unread badges or notification previews. They don't need full dynamics sections unless the story moves into them.

**Juilliard Cohort** (iMessage, ~12-15): Graduating class. More musical content. Quieter since graduation. Activates when someone books a concert or gets gig.

**Crawford Extended** (iMessage, ~8-10): Tommy's wider family — parents, siblings, cousins. Logistical. Alex treated as family, posts like nephew.

**Keeneland / Horse People** (iMessage/WhatsApp, ~10-15): Seasonal (Oct peak). Woodford County horse world. Jake authority. Alex reads more than posts. When he posts, genuine knowledge.

**Westminster Music** (WhatsApp, ~6-8): Small group from Westminster music department. The serious ones. Shares recordings, concert links, instrument drama. Quieter. Activates around concerts.

**Walker Holdings** (Slack workspace): Family business. Alex in relevant channels: #general (low volume, reads rarely posts), #alex-business (Eleanor, Nadia, Diane, Alex — operational core, Alex replies to decisions), #hatfield-ops (Alex dips in occasionally), #stables (feeding schedules, vet visits, short messages), #security (Kevin, security team, Eleanor, Nadia — Alex checks when traveling).

**The Stables** (WhatsApp, ~4-5): Alex, Tommy, and others who help with horses. Purely logistical. Feeding, vet, farrier, who's riding. Most unglamorous chat on his phone, therefore one of most real.

**LA People** (iMessage, ~25-30): LA isn't Alex's city. Business and obligation. Industry meetings Eleanor schedules, fittings, Legacy overlap, occasional dinner. Loose coalition rather than tight friends. Requires more lead time — LA requires driving.

**God-siblings** (iMessage, ~5-6): Apple Martin, Moses Martin, Zachary/Elijah Furnish-John, Alex, possibly one or two others. Irregular but warm. Childhood family friends through parents, not school or geography. Activates around family gatherings or when parents' schedules overlap.

**Dormant chats:** Every phone has them. Old Westminster chats. One-off villa chat from two summers ago. Juilliard chamber group chat. Charity event planning chat finished. These show up as grey, unread, low on list. They're texture — Alex scrolls past them.

---

## RENDERING RULES FOR ALL CHATS

**Use phone-renderer skill for formatting.** This file tells WHAT is on screens (who posts, in what voice, with what energy). The skill tells HOW to format.

**Apply Voice Construction Rules** (NPC_VOICE_GUIDE.md §X): A voice card is starting point, not boundary. Not every character repeats their signature trait every message. Build from context. Let characters be more than one thing per scene.

**Group chats are ensemble scenes:** No character dominates with their one trait. A good chat message from Maude is observational *sometimes* and something completely different other times. Feel like a room of actual people, not lineup of catchphrases taking turns.

**No chat echo:** Don't repeat the same jokes or references every time. "NOT Cody" is funny once or twice a session, not every scene.

**Information walls are absolute:** If a character doesn't know something, they can't reference it. What they know shapes their voice.

**Information isolation in cut scenes:** Cut-scene chats (The Circle Inner, Eleanor + Nadia, Legacy Girls, Legacy Elders, Dawson Family Proper, Industry Back-Channels, Tommy + Jake) are invisible to Alex. He cannot see, reference, or react to anything said there unless someone tells him directly.
