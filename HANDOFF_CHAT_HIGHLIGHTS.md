ACTIVE_RUNTIME_SUMMARY
```yaml
doc: HANDOFF_CHAT_HIGHLIGHTS.md
version: 1
runtime_first: true
session_date: 2026-04-09
doc_type: session_highlights
priority_scan:
  - repeat_error_prevention
  - design_principles
  - information_asymmetry
source_last_updated: "Session 1 (project date: Thursday, April 9, 2026)"
corrections: 6
runtime_generated_on: 2026-04-14
```

ARCHIVE_APPENDIX
> **What this is:** Key exchanges, corrections Ryan made during the session, and design principles established through dialogue. Prevents the next Claude from repeating errors. Append each session.

---

# ALEX WILSON WORLD v5 — SESSION HIGHLIGHTS

---

## CORRECTIONS RYAN MADE (CARRY FORWARD — THESE PREVENT REPEATS)

| Error | Correction | File that fixes it |
|-------|-----------|-------------------|
| Assumed all Claude Chat Project files always load into context | Ryan: "You might want to do some research. Claude does use RAG if your project files hit a certain threshold." RAG activates at ~13 files, all-or-nothing — once active, ALL files go through RAG. | INDEX.md + project instructions field architecture |
| Assumed RAG only hit files after the 12th | Ryan confirmed: "Does the RAG kick in on files AFTER the 12 or on all files if you have more than 12?" — confirmed all files go through RAG once the threshold is hit | NARRATOR.md §RAG ARCHITECTURE |
| Planned to consolidate to ~12 files to avoid RAG | Ryan's correction led to redesign: design FOR RAG rather than fighting it — focused topically pure files + INDEX.md + rich project instructions field | Entire v5 architecture |
| Kentucky defaulting to Appalachian coding | Ryan: explicitly flagged as "FAILURE MODE 1 — KENTUCKY TRAP." Woodford County is Surrey, not Appalachia. | WOODFORD.md, PROJECT_INSTRUCTIONS_FIELD.md |
| Discovery/newly famous defaulting for Alex | Ryan: "FAILURE MODE 2 — DISCOVERY TRAP." Alex has been famous his entire life. | SCALE.md, PROJECT_INSTRUCTIONS_FIELD.md |
| Brooding/pensive personality defaults | Ryan: "FAILURE MODE 3 — TORTURED ARTIST TRAP." Alex is warm, funny, charming, confident. | ALEX_CHARACTER.md (positive anchor) |

---

## KEY DESIGN PRINCIPLES ESTABLISHED THROUGH DIALOGUE

**On file size:** "The problem is Claude has to go back to the files for a refresh/update — this means it has to load a significantly large file again." → Smaller focused files are better for mid-session re-referencing.

**On INDEX.md:** "I'd go more specific smaller files BUT we make better use of project instructions, maybe also creating an INDEX.md file that contains a list of every file and what it does and write an instruction to tell Claude to review it first?" → INDEX.md as always-retrieved anchor.

**On what to build:** "My feeling is you create a folder called Alex Wilson v5. Build it out from what we've got without losing data." → Full migration, no data loss, new architecture.

**On the big question:** "So before we dive in — my big question — do we fix the files we have or design a complete new structure from the ground up. Keep the content/story but restructure to better work within what works best with Claude Chat." → Complete new structure.

**On Kentucky:** "OK good. Yes. But also we do need some local moments. When home he'd go to a bar in Lexington with friends, go fishing, go to Keeneland race course. He'd fly out of Bluegrass FBO." → Local moments are important; WOODFORD.md explicitly includes these.

**On ALEX_CATALOG.md:** Ryan confirmed this should NOT be in project knowledge. "Its meant to be just for some sessions when I decide to run the songwriter scenario, and even then I like to drop specific songs to push him into one genre or even multiple genres."

---

## INFORMATION ASYMMETRY TABLE

*This section tracks what different parties know about each other in the story world. Critical for preventing information bleed between sessions.*

| Information | Who Knows | Who Doesn't Know |
|-------------|-----------|-----------------|
| Alex's exact personal net worth (~$480-500M) | Eleanor, Edward Cahill, Judith Ansley, Alex (roughly) | Tommy, Sayre Boys, London Lot, general public, press |
| The Rule (nothing released until graduation) | Inner circle (Rosie, Homer, Eleanor, Tommy, The Circle) | Industry (knows there's a rule but not from whom it came), general public |
| Alex's ghostwriting credits and which songs | Alex, Eleanor | Tommy, Sayre Boys, London Lot, press, general public |
| Alex's biological father situation / Dawson reconnection | Alex, Rosie, Homer, Eleanor | Tommy (broadly aware but not details), others (unaware) |
| Walker Holdings total valuation (~$18-20B) | Eleanor, inner family | Public (no Forbes list), industry (estimates), Tommy (doesn't think about it) |
| The cascade viral moment context (what it means for career) | Eleanor (fully), Alex (partly — he knows it happened, doesn't know exact scale) | General public (sees the fame, not the infrastructure reality) |

---

## RUNNING NOTES ON RYAN'S PREFERENCES

- **He wants LOCAL moments in Kentucky** — not just global glamour. Keeneland, Hatfield Lexington, fishing, Bluegrass FBO are important.
- **He cares about detail** — "Can you build all of that without losing any detail?" The answer is always yes, preserve everything.
- **He wants files to be Claude-efficient** — smaller, focused files that retrieve accurately mid-session are preferred over large omnibus documents.
- **He uses handoffs** — the story-handoff skill is established. He ends sessions with handoffs and starts new chats from them.
- **He starts new chats within the project** for different expansion tasks — the v5 folder is the permanent base, new chats extend specific areas.

---

*Last updated: Session 1 (project date: Thursday, April 9, 2026)*
