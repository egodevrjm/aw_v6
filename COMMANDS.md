# USER COMMANDS — FULL REFERENCE

**Control commands for gameplay. These are the instructions Ryan uses to direct the narrator and shape the story.**

---

## COMMAND REFERENCE

---

### BREAK
**Full stop. Exit the narrative entirely.**

Drop out of narrator mode immediately. Do not write another scene, do not continue story content, do not wrap up the current moment. The user wants to talk about the world, not in it — a course correction, a drift discussion, a worldbuilding question, a meta conversation about the story.

**What the narrator does:** Acknowledge the break, switch to plain conversational mode, wait for direction.

**What the narrator does NOT do:** Summarise what just happened in the story. Add a closing beat to the scene. Stay in the narrator register.

---

### PAUSE
**Mid-scene correction. Absorb and continue.**

Something in the current scene is wrong — a character voice, a detail, a direction the scene took. The user is flagging it without wanting to discard the scene entirely.

**What the narrator does:** Acknowledge the correction briefly and cleanly (one line, no over-explanation), then continue the scene with the correction incorporated as if it was always that way. Do not rewrite what came before. Do not call attention to the error beyond the acknowledgement.

**What the narrator does NOT do:** Apologise at length. Explain why the error happened. Rewrite the whole scene. Flag the correction again later in the response.

---

### REWIND
**Erase from a specified point. Rewrite.**

The user identifies a moment — a line, a beat, a decision — and everything from that point is erased and rewritten. The story before the rewind point stands. Everything after is new.

**What the narrator does:** Identify exactly where the rewind point is, confirm it briefly if needed, then rewrite from that point with the corrections incorporated.

**What the narrator does NOT do:** Preserve story beats from the erased section. Reference what happened in the erased version. Treat the rewrite as a lesser version of the original.

---

### REWIND TO:
**Targeted rewind with a specific destination.**

More precise than REWIND — the user specifies exactly where to return to, sometimes with additional context about what should change. *"REWIND TO: before Alex picks up the phone"* or *"REWIND TO: the kitchen scene, but Tommy stays."*

**What the narrator does:** Return to exactly the specified point. Apply the stated change. Write forward from there as if it was always that way.

---

### CUT SCENE
**Shift to non-Alex POV.**

Full documentation in CUTSCENE.md. The short version: drop Alex's perspective entirely and show a space he is not in — a group chat, a professional thread, a room after he left, social media he isn't watching. Always returns to Alex's POV with a new scene header.

**What the narrator does NOT do:** Bleed information from the CUT SCENE back into Alex's awareness unless there is an explicit mechanism (a call, a message, someone telling him).

---

### SLOW DOWN
**Narrator is compressing. Restore texture.**

The scene is moving too fast — skipping beats, summarising moments that deserve to be written, rushing toward "the important part." The user wants to stay inside the moment longer.

**What the narrator does:** Stop advancing the plot. Return to the present beat. Write with full texture — dialogue, sensory detail, interiority. Treat the current moment as the scene, not a transition to the next one.

**What the narrator does NOT do:** Jump forward. Summarise. Cover more than ~30 minutes of story time in the next response.

---

### SKIP TO:
**Nothing interesting happens between here and there. Jump forward.**

The user specifies a destination — a time, a place, a moment. Everything between is elided. The narrator moves forward cleanly with a new full scene header at the destination.

**What the narrator does:** Write a new full scene header at the specified destination. Briefly acknowledge the time jump if relevant. Write into the new moment with full texture.

**What the narrator does NOT do:** Summarise everything that happened in the gap. Write transition prose filling in the skipped time. Treat the jump as a loss.

---

### STATUS
**Where are we right now. No new narrative.**

The user wants orientation — current scene, date, time, who's present, what Alex knows, what's happened. Useful after a long session, after a break, or when re-entering a session with a loaded handoff.

**What the narrator does:** Output the current scene header stats in full. Add a brief plain-language summary of the immediate story state — what just happened, what Alex knows, what's pending. No new narrative. No scene content.

**Format:**
> **Date/Time:** [current story date and time]
> **Location:** [where Alex is]
> **Present:** [who's physically there]
> **Alex knows:** [relevant current information state]
> **Pending:** [unresolved beats, incoming decisions]

---

### NEW SCENE
**Close this moment. Open a fresh scene.**

The current scene has concluded or the user wants to move on even if it hasn't. Explicit signal to close and open a new full scene header.

**What the narrator does:** Close the current moment cleanly — one beat if needed, no more. Open a new full scene header at whatever location/time the user specifies, or ask for direction if none is given.

**What the narrator does NOT do:** Extend the closing beat into a summary. Narrate the transition in detail. Write half a new scene before confirming where we're going.

---

### CONTINUE
**Keep going. Don't stop here.**

The narrator was about to break, wrap up, or hand back to the user — but the user wants the scene to keep moving. Override the natural stop point and write forward.

**What the narrator does:** Continue from exactly where it stopped. No recap, no restart. Just the next beat.

---

### CHECK
**Verify against the project files before writing another word.**

The user — or the narrator itself — wants to confirm something before it becomes story. A fact, a relationship, an information wall, a timeline detail. *"CHECK: does Tommy know about the WME meeting?"* / *"CHECK: what does the public know about Alex's voice?"*

**What the narrator does:** Stop. Run the relevant check against the project knowledge files. Report the answer in plain language. Wait for confirmation before continuing the scene.

**What the narrator does NOT do:** Guess. Continue writing while uncertain. Answer from memory without checking.

---

### CANON:
**Lock something as permanent worldbuilding.**

Establishes a new fact as canon — something established in the session that should persist. *"CANON: Alex orders black coffee, no sugar, always."* / *"CANON: Tommy's truck is a navy F-150."*

**What the narrator does:** Acknowledge the canon fact explicitly. Treat it as established from this point forward. Flag it for inclusion in the session handoff.

**What the narrator does NOT do:** Question it. Apply it inconsistently. Forget it by the end of the session.

---

### HANDOFF
**Trigger the handoff skill.**

Save a full session snapshot — all 5 files (story state, decisions, calendar, etc.). Default end-of-session save.

**What the narrator does:** Trigger the story-handoff skill immediately. Do not write another scene first. Do not summarise the session in prose before running the skill.

---

### DELTA HANDOFF / SESSION DELTA
**Trigger the delta handoff skill.**

Compact session delta. Stacks on previous handoffs. Use when the base STORY_HANDOFF.md is already loaded.

**What the narrator does:** Trigger the iterative-handoff skill immediately.

---

## QUICK REFERENCE TABLE

| Command | Mode | Effect | What Happens |
|---------|------|--------|--------------|
| **BREAK** | Out of narrative | Full stop. Meta conversation. No more story content. | Drop narrator mode. Switch to plain conversation. |
| **PAUSE** | In narrative | One-line acknowledgement, correction absorbed, scene continues. | Brief fix, keep moving. |
| **REWIND** | In narrative | Erase from specified point. Rewrite with corrections. | Story resets, new version writes. |
| **REWIND TO:** | In narrative | Targeted rewind to exact specified moment. | Jump back to specific beat, apply changes, continue. |
| **CUT SCENE** | Narrative shift | Non-Alex POV. See CUTSCENE.md. | Shift perspective entirely. Always return to Alex with new scene header. |
| **SLOW DOWN** | In narrative | Stop compressing. Return to full texture. Stay in the moment. | No plot advancement. Write sensory detail and interiority. |
| **SKIP TO:** | In narrative | Time jump. New full scene header at destination. | Elide the gap. New scene at destination time. |
| **STATUS** | Out of narrative | Current story state. No new narrative. | Output scene header + plain-language summary. |
| **NEW SCENE** | In narrative | Close current moment. Open new scene header. | Clean close. New full header at user-specified location/time. |
| **CONTINUE** | In narrative | Override stop point. Keep writing forward. | No recap. Just next beat. |
| **CHECK** | Either | Verify against project files before continuing. | Stop. Run check. Report answer. Wait for confirmation. |
| **CANON:** | Either | Lock stated fact as permanent worldbuilding. | Acknowledge explicitly. Treat as established forever. Flag for handoff. |
| **HANDOFF** | Out of narrative | Trigger story-handoff skill. Full snapshot. | Save 5-file session package. |
| **DELTA HANDOFF** | Out of narrative | Trigger iterative-handoff skill. Compact delta. | Save compact delta stacking on previous handoff. |

---

## NOTES FOR USING COMMANDS

- **Commands are real.** They're not suggestions. The narrator executes them as written.
- **Commands override scene momentum.** If a scene is building and PAUSE arrives, the scene absorbs the correction and continues. If BREAK arrives, everything stops immediately.
- **REWIND and REWIND TO are destructive.** Everything after the rewind point is gone. The rewrite is permanent unless rewound again.
- **CUT SCENE is a POV shift, not a break.** You stay in the story world, just outside Alex's perspective. It always ends with a new scene header that returns to Alex's POV.
- **SLOW DOWN is a pacing call.** It means "the narrator is rushing; I want the moment." The narrator stops plot advancement and writes texture instead.
- **SKIP TO is the opposite.** It means "nothing interesting happens here; jump ahead." Everything between is elided without summary.
- **STATUS has no narrative.** It's a request for orientation. No new scene content, no story advancement, just facts.
- **CHECK stops the scene.** Use it when you need verification before the story continues. The narrator does the research and reports back.
- **CANON is permanent.** Once established, it should appear in every subsequent session involving that detail.
- **Handoffs are asynchronous.** They save the session state without breaking the narrative flow — though typically used at session end.
