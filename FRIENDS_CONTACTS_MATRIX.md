# FRIENDS_CONTACTS_MATRIX — CROSS-CHAT CONTACT MAP (v1)

**Answer:** Yes — we should keep a dedicated friends/contacts list keyed by chat code. It gives the model a single source of truth for who belongs where and sharply reduces cross-chat bleed.

**Scale:** v2 now carries a hundreds-scale directory (288 roster rows) combining canonical memberships and brainstorm extensions across family, school friends, famous peers, and legacy networks.

This file is a **normalized membership map** that complements `VOICES_CHATS.md` (tone/dynamics) and `GROUP_CHAT_ARCHITECTURE.md` (rendering protocol).

---

## Chat Code Key

- `FAM` = Family
- `SB` = Sayre Boys
- `LL` = London Lot
- `WB` = Westminster Boys
- `NYL` = New York Lot
- `LA` = Legacy Admissions
- `SH` = Summer House
- `LT` = La Terrazza
- `PH` = Phoenix Hollow
- `DC` = Dawson Cousins

---

## Membership Confidence Key

- `C` = Canonical (explicitly named in existing files)
- `P` = Probable (strongly implied, but not explicit membership line)
- `B` = Brainstorm candidate (not yet canon; add only if desired)

---

## Canonical/Probable Contact Matrix (Seed)

| Person | Primary circle | Chats | Conf | Notes |
|---|---|---|---|---|
| Alex Wilson | Core | FAM, SB, LL, WB, NYL, LA, SH, LT, PH, DC | C | Cross-world bridge |
| Rosie Walker | Family/Circle | FAM, PH | C | Family + compound anchor |
| Homer Wilson | Family/Circle | FAM, PH | C | Low-volume texter |
| Eleanor Vance | Family/Operations | FAM, PH | C | Operational voice |
| Tommy Crawford | Sayre | SB | C | Alex's closest friend |
| Cody Ashford | Sayre | SB | C | Highest SB volume |
| Jake Patterson | Sayre | SB | C | Sparse, practical |
| Danny Harlan | Sayre | SB | C | Late-thread precision |
| Dom Reyes | Sayre | SB | P | Listed in Sayre profiles; include if active |
| Freddie Ashworth | London | LL, WB | C | Shared LL/WB overlap |
| Hugo Manners | London | LL, WB | C | Shared LL/WB overlap |
| Cosima Hicks | London | LL | C | Core LL voice |
| Jess Okonkwo | London | LL | C | Music discovery voice |
| Jonathan Dawson | London | LL | C | Quiet and surgical |
| Lucas Ashby | London | LL | C | Architecture/buildings angle |
| Archie Cadogan | Westminster | LL, WB | C | Loud in WB |
| Rufus King | London/Equestrian | LL, WB | C | Horses/polo bridge |
| Amelia Windsor | London | LL | C | Royal-adjacent |
| Samuel Chatto | London | LL | C | Arts/ceramics texture |
| Arthur Chatto | London | LL | C | Royal-adjacent |
| Flora Ogilvy | London | LL | C | Royal-adjacent |
| Cara Delevingne | London | LL | C | Drop-in chaotic energy |
| Adwoa Aboah | London | LL | C | Fashion-cultural voice |
| Raye | London | LL | C | Music/event layer |
| Rafferty Law | London | LL | C | London social crossover |
| Tom Holland | London | LL | C | Occasional friendly presence |
| Iris Law | London | LL, LA | C | London + Legacy crossover |
| Lila Moss | London | LL, LA | C | London + Legacy crossover |
| Rocco Ritchie | London | LL, LA | C | London + Legacy crossover |
| Lennon Gallagher | London | LL | C | London social scene |
| Anaïs Gallagher | London | LL | C | London social scene |
| Nora Yoon | NYC/Juilliard | NYL | C | Core NYL driver |
| Marcus Delacroix | NYC/Juilliard | NYL | C | Core NYL driver |
| Derrick Washington | NYC/Juilliard | NYL | C | Late-night NYL |
| Sasha Volkov | NYC/Juilliard | NYL | C | Juilliard circle |
| Jin Park | NYC/Juilliard | NYL | C | Juilliard circle |
| Sam Okafor | NYC | NYL | C | Juilliard-club bridge |
| Henry Cabot | NYC | NYL | C | Table/venue organizer |
| Naia Reyes | NYC | NYL | C | NYL social layer |
| Timothée Chalamet | NYC | NYL | C | NYC famous layer |
| Zoë Kravitz | NYC/Legacy | NYL, LA | C | Cross-coast bridge |
| Bella Hadid | NYC | NYL | C | NYL famous layer |
| Gigi Hadid | NYC | NYL | C | NYL famous layer |
| Dev Hynes | NYC | NYL | C | Music layer |
| Robert Pattinson | NYC | NYL | C | NYC famous layer |
| Jeremy Allen White | NYC | NYL | C | NYC famous layer |
| Florence Pugh | NYC | NYL | C | NYC famous layer |
| Paul Mescal | NYC | NYL | C | NYC famous layer |
| A$AP Rocky | NYC | NYL | C | NYC famous layer |
| Maya Hawke | NYC/Legacy | NYL, LA | C | Strong crossover |
| Maude Apatow | Legacy | NYL, LA | C | NYC + Legacy crossover |
| Jack Schlossberg | Legacy | NYL, LA | C | NYC + Legacy crossover |
| Gracie Abrams | Legacy/Music | NYL, LA | C | NYC + Legacy crossover |
| Apple Martin | Legacy/Family-adjacent | LA, LT | C | Alex sibling-close |
| Moses Martin | Legacy/Family-adjacent | LA | C | Lower activity |
| Kaia Gerber | Legacy/LA | LA | C | LA anchor |
| Presley Gerber | Legacy/LA | LA | C | More sporadic |
| Noah Cyrus | Legacy | LA | C | Music content |
| Miley Cyrus | Legacy | LA | C | Bridge/current authority |
| Jaden Smith | Legacy | LA | C | Current active set |
| Willow Smith | Legacy | LA | C | Current active set |
| Lily-Rose Depp | Legacy | LA | C | Bridge/current set |
| Brooklyn Beckham | Legacy | LA | C | Bridge/current set |
| Romeo Beckham | Legacy | LA | C | Bridge/current set |
| Stella McCartney | Legacy founder | LA | C | Founder generation |
| Sean Ono Lennon | Legacy founder | LA | C | Founder generation |
| Nicole Richie | Legacy founder | LA | C | Founder generation |
| Kate Hudson | Legacy founder | LA | C | Founder generation |
| Riley Keough | Legacy bridge | LA | C | Bridge authority |
| Frances Bean Cobain | Legacy bridge | LA | C | Bridge authority |
| Dakota Johnson | Legacy bridge | LA | C | Bridge authority |
| Jack Quaid | Legacy bridge | LA | C | Bridge authority |
| Lenny Kravitz | Circle | PH | C | Compound regular |
| Madonna | Circle | PH | C | Compound occasional/regular |
| Uma Thurman | Circle-adjacent | PH | C | PH named member |
| Stevie Nicks | Circle | PH | C | Circle elder |
| Dolly Parton | Circle | PH | C | Circle elder |
| Elton John | Circle | PH | C | Circle elder |
| Paul McCartney | Circle | PH | C | Circle elder |
| Joni Mitchell | Circle | PH | C | Circle elder |
| Brandi Carlile | Circle | PH | C | Circle bridge generation |
| Beyoncé | Circle | PH | C | Solstice/compound presence |
| Adele | Circle | PH | C | Solstice presence |

---

## Brainstorm Additions (Not Canon Yet)

Use these only if you want to expand cast diversity. Keep them marked `B` until promoted.

| Person | Suggested circles | Reason |
|---|---|---|
| Session Musician Pool A/B/C | PH, SH | Improve non-famous texture in music-heavy chats |
| Compound Ops Contacts (grounds, events, transport) | PH | More realistic logistics layer |
| Sayre peripheral friends (2-4 names) | SB | Avoid over-reliance on the same 4 voices |
| London equestrian secondary names (2-3) | LL, WB | Increase horse/polo realism |
| NYC working-musician contacts (teaching/session) | NYL | Ground NYL in real working life |
| LA creator/operator contacts (assistants, stylists, producers) | LA | Reduce celebrity-only messaging |

---

## Maintenance Rules

1. Keep one row per person.
2. `Chats` must use chat codes only.
3. New names start as `B` unless explicitly canonical in source files.
4. If a person appears in output but not here, add them immediately with confidence flag.
5. Reconcile this file with `VOICES_CHATS.md` whenever rosters are updated.



---

## Extended Master Name Index (Hundreds-Scale Roster)

This section intentionally pushes into **hundreds of names** spanning famous people, old school friends, family, and legacy/nepo peers.

| Person | Segment | Chats (if any) | Conf |
|---|---|---|---|
| Barack Obama | famous/family-friend | PH | P |
| Michelle Obama | famous/family-friend | PH | B |
| Uma Thurman | famous/family-friend | PH | C |
| Lenny Kravitz | famous/family-friend | PH | C |
| Madonna | famous/family-friend | PH | C |
| Dave Grohl | famous/family-friend | PH | P |
| Rick Rubin | famous/family-friend | PH | P |
| Lady Gaga | famous/family-friend | PH | P |
| Chris Martin | family/godparent | PH, LT | P |
| Donatella Versace | family/godparent | - | P |
| Stella McCartney | family/godparent | LA | C |
| Elton John | family/godparent | PH | C |
| Arthur Russell | music-reference | - | B |
| Alicia Keys | music-network | PH | B |
| Bad Bunny | music-network | - | B |
| Billie Eilish | music-network | - | B |
| Harry Styles | music-network | - | B |
| Kendrick Lamar | music-network | - | B |
| Dua Lipa | music-network | LL | B |
| Caroline Polachek | music-network | NYL | B |
| Dom Sessa | friends | NYL | B |
| Dominic Sessa | friends | NYL | B |
| Barry Keoghan | friends | LL | B |
| Hailey Bieber | friends | LA | B |
| George Clooney | family-friend | PH | B |
| Jane Fonda | family-friend | PH | B |
| Jack White | music-network | PH | B |
| Eddie Vedder | music-network | PH | B |
| Jackie Kennedy Schlossberg | legacy-family | LA | B |
| Sarah Wilson | family | DC | P |
| Lady Sarah Wilson | family | DC | P |
| Lady Sarah Anne Dawson | family | DC | P |
| Lord Charles Dawson | family | DC | P |
| Beatrice Dawson | family | DC | C |
| James Dawson | family | DC | P |
| Margaret Ashworth | family-friend | LL | P |
| Lady Caroline Ashby | family-friend | LL | P |
| Lady Alice Pemberton | family-friend | LL | P |
| Lady Sophia Halford | family-friend | LL | P |
| Lady Louise Windsor | family-friend | LL | P |
| Lady Caroline | family-friend | LL | P |
| Louise Windsor | family-friend | LL | P |
| Sarah Chatto | family-friend | LL | P |
| Noah Patterson | old-school | SB | P |
| Brent Patterson | old-school | SB | P |
| Lydia Patterson | old-school | SB | P |
| Roy Harlan | old-school | SB | P |
| Kayla Crawford | old-school | SB | P |
| Darlene Crawford | old-school | SB | P |
| Jim Crawford | old-school | SB | P |
| Warren Ashford | old-school | SB | P |
| Trish Ashford | old-school | SB | P |
| Ethan Woods | old-school | SB | P |
| Henry Ashby | old-school | LL | P |
| Pippa Aldridge | old-school | LL | P |
| Nina Sherwood | old-school | LL | P |
| Peter Aldridge | old-school | LL | P |
| Rufus King | old-school | LL, WB | C |
| Naia Reyes | friends | NYL | C |
| Dev Hynes | friends | NYL | C |
| Robert Pattinson | friends | NYL | C |
| Jeremy Allen White | friends | NYL | C |
| Florence Pugh | friends | NYL | C |
| Paul Mescal | friends | NYL | C |
| Timothée Chalamet | friends | NYL | C |
| Bella Hadid | friends | NYL | C |
| Gigi Hadid | friends | NYL | C |
| AP Rocky | friends | NYL | P |
| A$AP Rocky | friends | NYL | C |
| Sasha Volkov | friends | NYL | C |
| Jin Park | friends | NYL | C |
| Nora Yoon | friends | NYL | C |
| Marcus Delacroix | friends | NYL | C |
| Derrick Washington | friends | NYL | C |
| Sam Okafor | friends | NYL | C |
| Henry Cabot | friends | NYL | C |
| Kaia Gerber | legacy | LA | C |
| Presley Gerber | legacy | LA | C |
| Kendall Jenner | legacy | LA | C |
| Kylie Jenner | legacy | LA | C |
| Jaden Smith | legacy | LA | C |
| Willow Smith | legacy | LA | C |
| Malia Obama | legacy | LA | C |
| Sasha Obama | legacy | LA | C |
| Lourdes Leon | legacy | LA | C |
| Hailie Jade Scott | legacy | LA | C |
| Ever Anderson | legacy | LA | C |
| Violet Affleck | legacy | LA | C |
| Seraphina Affleck | legacy | LA | C |
| Zahara Jolie | legacy | LA | C |
| Shiloh Jolie | legacy | LA | C |
| Vivienne Jolie | legacy | LA | C |
| North West | legacy | LA | C |
| Blue Ivy Carter | legacy | LA | C |
| Rumi Carter | legacy | LA | P |
| Sir Carter | legacy | LA | P |
| Archie Mountbatten-Windsor | legacy | LA | C |
| Lilibet Mountbatten-Windsor | legacy | LA | P |
| Sunday Rose Urban | legacy | LA | C |
| Faith Urban | legacy | LA | C |
| Elijah Hewson | legacy | LA | C |
| John Hewson | legacy | LA | C |
| Eve Hewson | legacy | LA | C |
| Damian Hurley | legacy | LA | C |
| Lennon Gallagher | legacy | LA, LL | C |
| Anaïs Gallagher | legacy | LA, LL | C |
| Destry Spielberg | legacy | LA | C |
| Sasha Spielberg | legacy | LA | C |
| Rumer Willis | legacy | LA | C |
| Tallulah Willis | legacy | LA | C |
| Scout Willis | legacy | LA | C |
| Harlow Madden | legacy | LA | C |
| Deacon Phillippe | legacy | LA | C |
| Ava Phillippe | legacy | LA | C |
| Zachary Furnish-John | legacy | LA | C |
| Elijah Furnish-John | legacy | LA | C |
| Jack Schlossberg | legacy | LA, NYL | C |
| Tatianna Schlossberg | legacy | LA | C |
| Sosie Bacon | legacy | LA | C |
| Riley Keough | legacy | LA | C |
| Zoë Kravitz | legacy | LA, NYL | C |
| Frances Bean Cobain | legacy | LA | C |
| Miley Cyrus | legacy | LA | C |
| Noah Cyrus | legacy | LA | C |
| Dakota Johnson | legacy | LA | C |
| Jack Quaid | legacy | LA | C |
| Lily Collins | legacy | LA | C |
| Billie Lourd | legacy | LA | C |
| Zelda Williams | legacy | LA | C |
| Margaret Qualley | legacy | LA | C |
| Scott Eastwood | legacy | LA | C |
| Lily-Rose Depp | legacy | LA | C |
| Brooklyn Beckham | legacy | LA | C |
| Romeo Beckham | legacy | LA | C |
| Domhnall Gleeson | legacy | LA | C |
| Colin Hanks | legacy | LA | C |
| Elizabeth Hanks | legacy | LA | C |
| Mamie Gummer | legacy | LA | C |
| Enrique Iglesias | legacy | LA | C |
| Wolfgang Van Halen | legacy | LA | C |
| Jason Bonham | legacy | LA | C |
| Rashida Jones | legacy | LA | C |
| Norah Jones | legacy | LA | C |
| Dhani Harrison | legacy | LA | C |
| Jakob Dylan | legacy | LA | C |
| Kate Hudson | legacy | LA | C |
| Nicole Richie | legacy | LA | C |
| Sean Ono Lennon | legacy | LA | C |
| Zoe Cassavetes | legacy | LA | C |
| Emma Chamberlain | la-creative | SH | C |
| Sabrina Carpenter | la-creative | SH | C |
| Jenna Ortega | la-creative | SH | C |
| Jacob Elordi | la-creative | SH | C |
| Tommaso Corsini | summer-core | LT | C |
| Edo Ferretti | summer-core | LT | C |
| Camille Aubert | summer-core | LT | C |
| Félix Arnoult | summer-core | LT | C |
| Lucía Montero | summer-core | LT | C |
| Giulia Agnelli | summer-core | LT | C |
| Maya Hawke | summer-core | LT, LA, NYL | C |
| Gracie Abrams | summer-core | LT, LA, NYL | C |
| Apple Martin | summer-core | LT, LA | C |
| Moses Martin | summer-core | LA | C |
| Stevie Nicks | circle | PH | C |
| Dolly Parton | circle | PH | C |
| Elton John | circle | PH | C |
| Paul McCartney | circle | PH | C |
| Joni Mitchell | circle | PH | C |
| Brandi Carlile | circle | PH | C |
| Beyoncé | circle | PH | C |
| Adele | circle | PH | C |
| David Gilmour | circle | PH | P |
| Lucas Ashby | family-friend | DC, LL | C |
| Jonathan Dawson | family-friend | LL | C |
| Freddie Ashworth | family-friend | LL, WB | C |
| Hugo Manners | family-friend | LL, WB | C |
| Cosima Hicks | family-friend | LL | C |
| Jess Okonkwo | family-friend | LL | C |
| Archie Cadogan | family-friend | LL, WB | C |
| Samuel Chatto | family-friend | LL | C |
| Arthur Chatto | family-friend | LL | C |
| Flora Ogilvy | family-friend | LL | C |
| Amelia Windsor | family-friend | LL | C |
| Raye | family-friend | LL | C |
| Adwoa Aboah | family-friend | LL | C |
| Cara Delevingne | family-friend | LL | C |
| Tom Holland | family-friend | LL | C |
| Cody Ashford | old-school | SB | C |
| Jake Patterson | old-school | SB | C |
| Danny Harlan | old-school | SB | C |
| Tommy Crawford | old-school | SB | C |
| Dom Reyes | old-school | SB | P |
| Alex Wilson | core | FAM, SB, LL, WB, NYL, LA, SH, LT, PH, DC | C |
| Rosie Walker | core-family | FAM, PH | C |
| Homer Wilson | core-family | FAM, PH | C |
| Eleanor Vance | core-family | FAM, PH | C |
