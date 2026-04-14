# RETRIEVAL CONTRACT

Single source of truth for retrieval behavior across this project.

## 1) Minimal Mandatory Load Rules

For every prose scene, load these before writing:

1. `INDEX.md` (for routing only).
2. Scene location file (exact property/city file).
3. Character profile file(s) for every on-page character.
4. Character voice file(s) for every speaking character.
5. Any domain file required by the active activity (business/media/music/phone/chat/etc.).
6. `FACTS_LEDGER.md` whenever using numbers, counts, valuations, timelines, or date cutovers.

Minimum floor (never skip): **location + present-character files**.

## 2) Scene-to-File Mapping

Use this mapping in addition to the mandatory rules above.

| Scene context | Primary files |
|---|---|
| Compound morning/day-to-day | `COMPOUND.md`, `ALEX_CORE.md` |
| Compound studio/music work | `COMPOUND.md`, `ALEX_MUSIC.md`, `HOMER.md` |
| Hatfield's Lexington | `HATFIELD_BAR_GRILL.md`, `WOODFORD.md` |
| The Stave (London/NYC) | `HATFIELD_STAVE.md`, plus `LONDON.md` or `NYC.md` |
| Distillery / Still House dinner | `HATFIELD_DISTILLERY.md`, `HATFIELD_STILL_HOUSE.md`, `WOODFORD.md` |
| NYC residence/social | `NYC.md`, relevant cast files |
| London residence/social | `LONDON.md`, relevant cast files |
| Sardinia / summer circuit | `SARDINIA.md`, `SUMMER.md`, `LEGACY_SUMMER.md` |
| Business/strategy with Eleanor | `ELEANOR.md`, `WALKER_HOLDINGS.md` |
| Group chat scene | `VOICES_CHATS.md`, `GROUP_CHAT_ARCHITECTURE.md`, `FRIENDS_CONTACTS_MATRIX.md` |
| Phone render | `PHONE.md`, plus relevant `VOICES_*.md` |
| Media/press reaction | `MEDIA.md`, `SCALE.md`, `PUBLIC_PERCEPTION.md` |
| Cut scene (industry/public reaction) | `CUTSCENE.md` + relevant domain files |

## 3) Precedence and Conflict Rules

When sources disagree, resolve in this order:

1. **`FACTS_LEDGER.md`** for volatile numbers, dates, and cutovers.
2. **Topical canon files** (character/location/domain docs named for the subject).
3. **`INDEX.md`** for retrieval routing only (not canon detail override).
4. **`PROJECT_INSTRUCTIONS_FIELD.md`** for always-on narrator calibrations and behavior.

Tie-breakers:

- Newer explicit date-bound statements override older undated statements.
- Specific file beats general file (e.g., `HATFIELD_STAVE.md` beats umbrella business summaries for Stave details).
- If still unresolved, keep prose conservative, avoid inventing missing facts, and defer to the ledger/date-bound canon.
