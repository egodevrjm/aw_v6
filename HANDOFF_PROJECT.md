> **What this is:** Project build handoff — not a story session handoff. Captures what was built in the previous session and exactly what the next session should do. Load this into the new Claude Chat before starting work.

---

# ALEX WILSON WORLD v5 — PROJECT HANDOFF

**Session date:** Thursday, April 9, 2026
**Reason for handoff:** Context limit reached after completing full v5 migration. Next session goal: expand Hatfield Group and Walker Holdings content depth.

---

## WHAT WAS JUST BUILT

**Alex Wilson World v5** is a complete redesign of the interactive fiction project's document architecture, built to work correctly with Claude Chat Projects' RAG system.

### Why v5 Exists

Claude Chat Projects activates RAG (retrieval-augmented generation) at ~13 files — confirmed via Anthropic GitHub issue #25759. Once RAG is active, all files are retrieved selectively; none are guaranteed in context. v5 was designed for this:

- **48 topically pure files** named to match scene-query terms (e.g., `WOODFORD.md` retrieves when a scene is set in Woodford County)
- **Project instructions field** carries always-active calibrations (failure mode fixes, mandatory scene header format, structural rules) — this field is never RAG'd
- **INDEX.md** is effectively always retrieved because project instructions explicitly tell Claude to read it first

### v5 Folder Location

`Alex Wilson World v5/` — in Ryan's selected workspace folder on his computer.

**48 files total, ~11,700 lines.**

### Three Failure Mode Fixes Built Into Architecture

1. **KENTUCKY TRAP** → `WOODFORD.md` exists as a dedicated file. Woodford County = Surrey/Cotswolds with thoroughbred farms, not Appalachia. Named so it retrieves for any Kentucky scene.
2. **DISCOVERY TRAP** → `SCALE.md` carries the 12-section calibration + Redirect Principle. Mandatory BASELINE field in every scene header forces Claude to declare pap count and article volume before writing.
3. **TORTURED ARTIST TRAP** → `ALEX_CHARACTER.md` opens with a POSITIVE ANCHOR (who Alex IS: warm, funny, charming, sexually confident) before any "what he is not" content.

### Complete File List (48 files)

**Alex character:** ALEX_BACKGROUND.md, ALEX_CHARACTER.md, ALEX_CORE.md, ALEX_MUSIC.md, ALEX_PHYSICAL.md, ALEX_STYLE.md

**Key relationships:** ROSIE.md, HOMER.md, ELEANOR.md, TOMMY.md

**Supporting cast — full profiles:** CIRCLE.md, GODPARENTS.md, DAWSONS.md, SAYRE_BOYS.md, LONDON_LOT.md, LEGACY_SUMMER.md

**Voices — how characters speak:** VOICES_CORE.md, VOICES_CIRCLE.md, VOICES_SAYRE.md, VOICES_LONDON.md, VOICES_JUILLIARD.md, VOICES_CHATS.md

**Locations:** COMPOUND.md, WOODFORD.md, HATFIELD.md, NYC.md, LONDON.md, SARDINIA.md, LA.md

**Business & money:** WALKER_HOLDINGS.md, AW_HOLDINGS.md, AW_COLLECTION.md, STAFF.md

**Media & public world:** SCALE.md, MEDIA.md, PUBLIC_PERCEPTION.md, WIKIPEDIA.md

**Music world:** DISCOGRAPHY.md

**Summer & calendar:** CALENDAR.md, SUMMER.md

**Gameplay tools:** NARRATOR.md, COMMANDS.md, CUTSCENE.md, STARTER_SCENES.md, IMAGE_PROTOCOL.md, PHONE.md

**Navigation:** INDEX.md, PROJECT_INSTRUCTIONS_FIELD.md (not a knowledge file — contains content to paste into Claude Chat instructions field)

---

## WHAT'S THIN — THE NEXT TASK

Ryan's direction: **"build out Hatfield and friends."**

This means expanding the Hatfield Group and related Walker Holdings content into richer, more complete detail. The current `HATFIELD.md` exists but is structural — it has the framework without the texture.

### HATFIELD.md — Current State vs What's Needed

| Section | Current state | Needs |
|---------|--------------|-------|
| Hatfield Distillery | Good skeleton | More on distillery experience, cave program detail, visitor reality, Carolyn Hatfield-Moore profile |
| Hatfield Bar & Grill (Lexington) | Good | Menu texture, specific staff, Alex's specific behaviours there, regular crowd, physical detail |
| Hatfield Bar & Grill (other 11 locations) | One-line each | Real detail: what city, exact address area, year, notable crowd, any Alex connection |
| Hatfield Inns | Two lines | Full section: how many rooms, price point, design, which cities, what makes each one notable |
| The Stave — London | Thin | Full build: Soho address area, membership process, layout, the listening room specifications, who the members are, Alex's actual use of it |
| The Stave — NYC | Barely mentioned | Same treatment |
| Still House Restaurant (Bardstown) | One line | Full restaurant profile: cuisine style, who dines there, James Beard connection, specific dishes, chef |
| Limestone Springs | One line | More detail |
| Walker Wines | One line in Hatfield | Full wine catalog is in `Walker Wines Catalog.md` (v3 source) — content should be in HATFIELD.md or its own file |
| Hatfield Provisions | One line | Expand: which products, where sold, retail presence |

### Walker Wines — Specific Task

The Walker Wines catalog has 4 wines that need full profiles in v5. The source is `Walker Wines Catalog.md` in the v3 folder. The wines are:
- **The Hollow** — red
- **Radio Silence** — red
- **A Still Small Voice** — white
- **Starlight & Steel** — probably sparkling or rosé

Each needs: grape varieties, profile notes, production, price point, where it's sold, what Alex's relationship to it is.

### "Friends" — Possible Interpretations

Ryan said "Hatfield and friends" — this likely means:
1. Hatfield Group in full detail (above)
2. Possibly expanding `WALKER_HOLDINGS.md` with more operational texture
3. Possibly adding a dedicated `WALKER_WINES.md` if the Walker Wines content is rich enough to stand alone
4. Possibly adding detail on characters connected to Hatfield (Carolyn Hatfield-Moore, David Buckner — these people exist as names but have no profile)

**Ask Ryan to confirm scope** before diving deep — "friends" could mean expanding connected characters or it could mean the business empire's subsidiary operations.

---

## DESIGN PRINCIPLES — CARRY THESE FORWARD

1. **Ownership-first for venue/business files:** Alex enters Hatfield Bar & Grill the way someone enters a room their family owns — not as a celebrity visiting a business. Lead with his relationship, not the venue's features.

2. **Eleanor as machine operator, not solo actor:** Walker Holdings has staffed operations. David Buckner runs Hatfield Group day-to-day. Eleanor sits on the board for oversight. She doesn't manage the menu.

3. **Homer's one contribution:** Homer specified the listening room at The Stave. That's the only Hatfield operation he touched. Everything else is professionally managed. Protect this — don't expand Homer's operational involvement.

4. **Kentucky calibration:** Bardstown (where the distillery is) is bourbon country, not Appalachia. Horse country. Professional industry. The Still House restaurant is James Beard-nominated — it's not a roadside diner.

5. **Topically pure files:** If Walker Wines content is substantial, create `WALKER_WINES.md` as its own file rather than stuffing it into HATFIELD.md. RAG retrieves better from focused files.

6. **INDEX.md must be updated last** after any new files are created, to include the new files in the table.

---

## WORKING CONTEXT NOTES

**Source files for Hatfield expansion (all in Alex Wilson World v3/):**
- `HATFIELD.md` — v3 version may have more detail than v5
- `Walker Wines Catalog.md` — the 4-wine catalog with full tasting notes
- `WALKER_HOLDINGS_ORG.md` — org chart may have Hatfield division detail
- `PEOPLE_AND_WORLD.md` — may have staff names or Hatfield connections

**v5 files that cross-reference Hatfield:**
- `WALKER_HOLDINGS.md` — Hatfield Group overview numbers
- `WOODFORD.md` — covers Hatfield Lexington as a local venue
- `ALEX_CORE.md` — may reference bourbon knowledge

**Do not create:**
- `SONGWRITER_RULES.md` — session-drop document, not permanent project knowledge
- `ALEX_CATALOG.md` — song history catalog, confirmed excluded from v5

---

## HOW TO START THE NEW SESSION

Paste the following into the new chat to orient Claude before starting:

---

> **Project context:** I'm building Alex Wilson World v5 — an interactive fiction world-building project. We just completed a full 48-file migration from v3 to v5. The v5 folder is my selected workspace. The next task is to expand the Hatfield Group content in depth.
>
> **Files available to read:** The v5 folder contains HATFIELD.md (current thin version), WALKER_HOLDINGS.md (has Hatfield Group financial overview), WOODFORD.md (has Lexington local context). The v3 folder (also in workspace) contains the original source files including Walker Wines Catalog.md.
>
> **Design principles:** (1) Ownership-first — Alex uses Hatfield as family-owned space, not as a customer. (2) Eleanor oversees Hatfield board but David Buckner runs it. (3) Homer's only contribution was the listening room at The Stave. (4) Bardstown/Kentucky is professional bourbon country, not rural.
>
> **Ask me first:** What specifically do you mean by "friends" in "Hatfield and friends" — other Hatfield divisions, Walker Wines as a separate file, or expanding connected characters?

---

*Last updated: Session 1 (project date: Thursday, April 9, 2026)*
