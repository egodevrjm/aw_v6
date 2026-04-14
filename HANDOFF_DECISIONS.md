ACTIVE_RUNTIME_SUMMARY
```yaml
doc: HANDOFF_DECISIONS.md
version: 1
runtime_first: true
session_date: 2026-04-09
doc_type: architecture_decisions
priority_scan:
  - binding_architecture
  - binding_character_world
  - open_questions
source_last_updated: "Session 1 (project date: Thursday, April 9, 2026)"
open_questions: 4
binding_decisions: 18
runtime_generated_on: 2026-04-14
```

ARCHIVE_APPENDIX
> **What this is:** Architectural decisions made during the v5 build. These are binding choices — carry them forward. Add new decisions from each subsequent build session.

---

# ALEX WILSON WORLD v5 — ARCHITECTURE DECISIONS

---

## FILE ARCHITECTURE DECISIONS

| Decision | Context | Status |
|----------|---------|--------|
| 48 files instead of consolidated ~12 | RAG activates at ~13 files in Claude Chat Projects (confirmed Anthropic GitHub #25759). Once active, all files go through RAG. Smaller, topically pure files retrieve more accurately than large omnibus documents. | **Binding** |
| Project instructions field carries always-active calibrations | Three failure mode fixes, mandatory scene header format, ownership rules — these must be in context always. Instructions field never goes through RAG. | **Binding** |
| INDEX.md as guaranteed-first-retrieve | Project instructions explicitly instruct Claude to read INDEX.md first, making it effectively always in context despite RAG. INDEX must be updated every time a new file is added. | **Binding** |
| WOODFORD.md as dedicated Kentucky calibration file | The Kentucky Trap failure mode needed a dedicated file named "WOODFORD" so it retrieves accurately for any Woodford County / Kentucky scene. The fix is structural, not just written into a larger doc. | **Binding** |
| HATFIELD.md opens ownership-first | The v3 failure: HATFIELD.md wrote the venues as places Alex visits. v5 redesign: open with Alex's lifelong relationship to family-owned establishments. | **Binding** |
| ALEX_CHARACTER.md opens with positive anchor | Lead with who Alex IS (warm, funny, charming, confident) before any "what he is not" table. Training data pull toward Tortured Artist defaults; the positive anchor must come first. | **Binding** |
| ALEX_CATALOG.md NOT migrated to v5 | The song catalog is a session-drop document — Ryan drops specific songs for specific songwriter sessions. It is not permanent project knowledge and should not be in the knowledge files. | **Binding** |
| SONGWRITER_RULES.md NOT migrated to v5 | Session-drop document. Same reason. | **Binding** |
| VOICES_*.md files split by social circle | v3 had one large NPC_VOICE_GUIDE.md. v5 splits voice cards by group (Core, Circle, Sayre, London, Juilliard). Smaller files retrieve more accurately when only one group is in a scene. | **Binding** |
| PHONE.md as dedicated file | PHONE_WORLD.md from v3 was not covered by any v5 file. The email landscape table, notification calibration, and 3-layer narrator guidance are important for phone-rendered scenes. Created PHONE.md as a distinct file. | **Binding** |
| PROJECT_INSTRUCTIONS_FIELD.md is NOT a knowledge file | This file is Ryan's reference for what to paste into the Claude Chat instructions field. It does not get uploaded as project knowledge. | **Binding** |

---

## CHARACTER / WORLD DECISIONS

| Decision | Context | Status |
|----------|---------|--------|
| Eleanor is a machine operator, not solo actor | ELEANOR.md explicitly frames her as overseeing a professionally staffed enterprise. Walker Publishing (UMG admin deal), Hatfield (own CEO David Buckner), family office (12-15 staff), Greystone security (separate). Eleanor directs; she doesn't do. | **Binding** |
| Homer's only Hatfield contribution = listening room at The Stave | Homer specified the acoustic design of The Stave's listening room. That is his one contribution to any Hatfield operation. He does not consult on menus, operations, business decisions. | **Binding** |
| Rosie's origin story for Hatfield = one sentence | "Homer liked Hatfield whiskey. Rosie bought the distillery for him." That's it. Not a strategic acquisition. | **Binding** |
| Tommy is categorically different from all other friendships | Tommy predates all of Alex's fame. He is not impressed, not jealous, not ambitious. He reacts to scale (NetJets, Beyoncé at the table) not to comfort or wealth. He is the constant. | **Binding** |
| Alex's personal net worth = ~$480-500M, separate from Walker Holdings | Built from inherited capital (Sarah Dawson estate ~£10M, David Wilson estate ~$60M) and Walker distributions. Managed by Edward Cahill as Investment Director. NOT from family charity. | **Binding** |
| Post-cascade scale as default | Unless explicitly playing a PRE-CASCADE scene: 100M+ Spotify monthly listeners, 95M+ Instagram followers, 40-60+ articles/day globally, 120-180 paps on rotation across four cities. | **Binding** |
| The Rule is over as of May 22, 2025 | Alex graduated from Juilliard May 22, 2025. The Rule (nothing released, nothing promoted until graduation) is over. Eleanor held all industry calls for four years; they are now all returnable. | **Binding** |

---

## SCOPE DECISIONS (WHAT WAS INTENTIONALLY EXCLUDED)

| Excluded | Reason |
|----------|--------|
| ALEX_CATALOG.md | Session-drop document for songwriter scenarios |
| SONGWRITER_RULES.md | Session-drop document |
| phone-renderer-SKILL.md | Skill file, not project knowledge |
| skills/ directory | Skill infrastructure, not project knowledge |
| summer_calendar_2025.csv | Raw data; content folded into SUMMER.md and CALENDAR.md |
| PROJECT_INSTRUCTIONS_V4.md | Replaced by PROJECT_INSTRUCTIONS_FIELD.md in v5 |

---

## OPEN QUESTIONS / PENDING DECISIONS

| Question | Context | Status |
|----------|---------|--------|
| Should Walker Wines be its own file (WALKER_WINES.md) or stay in HATFIELD.md? | Walker Wines catalog has 4 wines with full tasting notes (from Walker Wines Catalog.md in v3). If content is rich, a dedicated file retrieves better for wine scenes. | **Open — ask Ryan** |
| What does "Hatfield and friends" include? | Ryan said to build out "Hatfield and friends" in the next session. "Friends" is undefined — could mean Hatfield subsidiary staff profiles (Carolyn Hatfield-Moore, David Buckner), Walker Holdings deeper content, or something else. | **Open — ask Ryan** |
| Carolyn Hatfield-Moore and David Buckner — full profiles needed? | Both are named in HATFIELD.md as Master Distiller and CEO respectively. Neither has a full character profile. | **Open** |
| Should WALKER_HOLDINGS.md have more operational texture? | Current version covers the business financials and org chart well. Could be expanded with more "day to day" feel. | **Open** |

---

*Last updated: Session 1 (project date: Thursday, April 9, 2026)*
