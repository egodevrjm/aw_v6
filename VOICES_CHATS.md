# VOICES_CHATS — ALL GROUP CHATS IN ALEX'S LIFE

**The complete reference for every group chat Alex participates in, cut-scene chats, texture-layer chats, and the technical rules for rendering them authentically. This file bridges the individual voice cards (NPC_VOICE_GUIDE.md and related files) with the group dynamics of how chats actually function.**

---

**Apply `GROUP_CHAT_ARCHITECTURE.md` before rendering any chat to enforce anti-conflation rules and speaker rotation.**

**Use `FRIENDS_CONTACTS_MATRIX.md` as the membership authority when there is any uncertainty about who belongs in which chat.**

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

## THE TEN ACTIVE CHATS

### FAM — Family (iMessage, 4 people)

**Members:** Alex, Rosie, Homer, Eleanor

**Tone:** Nobody performs. Fully direct. Shorthand built on a lifetime of knowing each other.

**How each posts:**
- **Rosie:** Photo of the garden at 7am, no caption. A single line from a song. A voice note from the porch — 45 seconds. Texts at irregular hours.
- **Homer:** Radio silence for days. Then one perfectly dry observation about something unrelated. *"The espresso machine is broken again."* More silence. *"Good."* (meaning: finally)
- **Eleanor:** Logistics, clearly labelled. *"Tuesday 11am call with WME. Yes or no."* Occasional warmth — birthdays, *"well done"* — but mostly operational.
- **Alex:** Checks daily. ❤️ to Rosie's photos. Actual replies to Eleanor's questions. *"ha"* to Homer's delayed non-sequiturs.

**What it actually looks like:** Tuesday morning. Rosie has sent a photo of the tobacco barn at dawn. Eleanor has sent a logistics thread. Homer has sent nothing in four days. Alex ❤️'s the photo, replies *"yeah"* to Eleanor's first item and *"you can handle the other two"* to the rest. By Wednesday Homer will say something perfect and completely unrelated to this thread.

**Alex's activity:** High. Daily. This is the core of his life.

---

### SB — Sayre Boys (iMessage, ~7)

**Members:** Tommy, Jake, Cody, Danny, Alex + 2-3 others from Woodford County money

**Tone:** The most relentless chat in Alex's life. Daily, without fail. Has been daily for five years — even when Alex was in London or New York. This chat kept the friendship alive across distance.

**How each posts:**
- **Cody:** Highest volume. Five texts where one would do. All caps when excited. *"I'M TELLING YOU RIGHT NOW—"* Reports on Woodford County events. First to post, last to drop a thread.
- **Tommy:** Short. Punchy. Usually funnier than Cody. *"No."* as complete response. *"Sure"* meaning it's happening.
- **Jake:** Barely posts. About horses, land, logistics. *"I'll drive."* No emoji. Nobody doubts him.
- **Danny:** One message per thread. Complete sentence. Arrives late, reads back, finds the exact right observation. *"That seems like it'll go well"* about a Cody plan (means it absolutely won't).
- **Alex:** More active than almost anywhere except FAM. Picks up Cody's energy, matches Tommy, drops something that makes everyone stop — usually from his world, landing absurd against Woodford County.

**Running jokes (use sparingly — once or twice per session max):**
- **"NOT Cody"** — the driving allocation, years-running
- **Keeneland** — fall pilgrimage planning (August-October)
- **"So how's [impossible person]?"** — Cody asking about Beyoncé, the Obamas, etc.
- **Lake weekends** — Jake's Herrington Lake house

**Real content (this is what fills most of the chat):**
- Work and daily life. Tommy at a construction site. Cody at his dad's place. Jake with a horse issue. The ordinary machinery of Woodford County life.
- Food. Where to eat, bourbon opinions, someone's mom cooked something.
- Sports. UK basketball especially. Bengals. NFL Sundays.
- Local news and gossip. Woodford County small-town drama.
- Weather, seasons, land. Flooding, frost, hay, creek levels.
- Cars and trucks. Opinions.
- Plans. Weeknight, weekend, who's doing what, watching the game somewhere.
- Alex's world, handled casually. Not every mention is a "how's Beyoncé" bit. Sometimes genuine: someone saw a pap photo, someone's girlfriend mentioned it, someone asks when he's back.

**Alex's role:** Often the audience for the Woodford County news cycle. Subject of gentle bewilderment without it being weird. Also just one of the boys — he has opinions about the Bengals, where to eat, about Cody's plans. When home, the chat is even more alive.

---

### LL — London Lot (WhatsApp, ~50-60)

**Members:** Freddie Ashworth (anchor), Jess Okonkwo, Cosima Hicks, Hugo Manners, Jonathan Dawson, Lucas Ashby, royal-adjacent people (Amelia Windsor, Samuel Chatto, Arthur Chatto, Flora Ogilvy), fashion/music/creative (Cara Delevingne, Adwoa Aboah, Raye, Rafferty Law, Tom Holland), equestrian crowd (Rufus King, Pippa Aldridge, Nina Sherwood), plus London-based famous people (Iris Law, Lila Moss, Rocco Ritchie, Lennon Gallagher, Anaïs Gallagher, and others from the broader London social scene)

**Tone:** Dry. Understated British register where "sounds fun" means definitely coming and "not sure I can make it" means definitely coming. Plans that sound vague are often quite fixed. Nobody announces things — things are suggested and then happen.

**The core driving voices (rotate, don't always feature all five):**
- **Freddie Ashworth:** Social engine. Posts a suggestion, it gains traction, twelve people are at the pub. Lowest drama, highest execution.
- **Hugo Manners:** Country weekends and polo. When he posts, the aristocratic countryside end activates.
- **Cosima Hicks:** Gallery openings, art world events. Dry about everything, right about most things six months before everyone agrees.
- **Jess Okonkwo:** Music events, RAM-adjacent, concerts the rest wouldn't have found. The musician.
- **Jonathan Dawson:** Quiet, complete sentences, occasional observation that makes people think. Won't post five times in a row.

**USE THE OTHER 25 PEOPLE — they should appear regularly:**
Archie Cadogan joins Freddie's plans loudly. Lady Amelia Windsor posts about fashion events. Samuel Chatto shares something about ceramics. Cara drops in from elsewhere, chaotic. Raye posts about a gig. Rafferty joins boys' plans. Tom Holland appears occasionally, friendly. Pippa and Nina bring the equestrian end. Every LL render should include at least one or two voices beyond the core five — not forced, just present.

**Real content (what fills most of the chat):**
- Restaurant and bar recommendations. Not just "anyone around Thursday" — specific opinions.
- Art, music, culture. Not just Cosima's gallery openings — someone saw something, someone's friend is in something.
- Fashion and events. Met, fashion weeks, galas. What to wear, discussed with British understatement.
- Weekend plans. London vs countryside. Hugo's place vs parents' place vs festival.
- Gossip — light, never vicious. Who's seeing whom, social mechanics.
- London logistics. Tube problems, weather, the comedy of the city.

**What it looks like on a normal week:** Hugo mentions a charity polo match. Cosima posts a gallery opening. Freddie asks if anyone is around Thursday. Archie immediately says yes. Cara drops in from Milan with something unrelated. By Thursday, a plan involving eight people has coalesced without anyone explicitly agreeing. Jonathan hasn't posted since Monday. Lucas sent something about a building. Amelia posted about dinner Saturday that three people quietly noted.

**Alex's role:** Gravitational centre without being loudest. When he's in London, the chat's activity roughly doubles. He drops into threads, doesn't start many. Occasionally puts a plan in motion — texts Nadia, she sorts it, he drops details in chat like it was nothing.

---

### WB — Westminster Boys (WhatsApp, ~10-12)

**Members:** Freddie Ashworth, Hugo Manners, Archie Cadogan, Rufus King, Alex, and 5-6 others from Westminster sixth form

**Tone:** Older, louder, more laddish than London Lot. School references nobody outside can access. Shorthand built over two years of sixth form that never updated.

**The register shift from LL:** Same people but unfiltered. Laddish where LL is dry. Loud where LL is quiet. School references are the barrier — if you weren't at Westminster, you can't follow half the conversation, which is partly the point.

**What it sounds like:** Inside jokes six+ years old. References to teachers, incidents, the specific geography of Westminster ("the green" / "that corridor" / nicknames for places that aren't their real names). Sporting fixtures and grudges that haven't expired. People are roasted here in ways they wouldn't be in LL.

**Real content:**
- Football. Properly. Opinions, matches, fantasy leagues, arguments.
- School memories as living reference. *"This is worse than when Archie [incident from 2019]"* — nobody explains, everybody gets it.
- Taking the piss out of each other. Relentless. Freddie about Hugo's country house pretensions. Hugo about Freddie's clothes. Archie about everything. Alex not exempt — the American-in-English-school thing is evergreen material.
- Plans that are rougher than LL plans. Not "shall we try that new place in Mayfair" — more "pub, 7, don't be late."
- Rufus and polo/horses.
- Girls — discussed frankly here in ways they wouldn't be in LL. Not vicious, but frank.

**Alex's role:** Was added first year at 16. Can access the references. One of the boys. His accent never stopped being funny to them and never will. Gets roasted about his world — it's affection coded as abuse, exactly like the Sayre Boys but in a British register.

---

### NYL — New York Lot (iMessage, ~40-50)

**Members:** Nora Yoon, Marcus Delacroix, Sasha Volkov, Jin Park, Derrick Washington (Juilliard peers), Zero Bond / Casa Cipriani regulars (Henry Cabot, Sam Okafor, Naia Reyes), plus NYC-based famous people (Timothée Chalamet, Zoë Kravitz, Bella Hadid, Gigi Hadid, Dev Hynes, Robert Pattinson, Jeremy Allen White, Florence Pugh, Paul Mescal, A$AP Rocky), plus NYC-based Legacy crossover (Maya Hawke, Maude Apatow, Jack Schlossberg, Gracie Abrams)

**Tone:** *"Tonight?"* Architecture of spontaneity. Plans form in under an hour. If not free tonight, someone else will be. NYC energy.

**The core driving voices (rotate them):**
- **Marcus Delacroix:** Announces things. Loud. *"CASA CIPRIANI. 9PM. NOT OPTIONAL."* It's optional but feels mandatory.
- **Nora Yoon:** Proposes actual things — concerts, recitals, Lincoln Center. Not just drinks, *something.*
- **Derrick Washington:** Late-night plans only. Never posts before 10pm. *"studio session, midnight, you know where."* Usually only two or three people but they're always right.
- **Sam Okafor:** The bridge between Juilliard world and club world. Knows everyone.
- **Henry Cabot:** Always has a table. *"I've got the corner at Zero Bond starting at 8."*

**USE THE OTHER 20 PEOPLE — they should appear regularly:**
Other Juilliard peers — someone sharing a concert they're playing, asking about a rehearsal space, announcing a gig. The Zero Bond / Casa Cipriani crowd — models, finance people, creatives. NYC-based Legacy crossover. Naia Reyes and other individual voices. Musical content — not just "studio session, midnight." Who heard what, who's playing where, a recording someone made.

**Real content:**
- Music. Actual discussion — not just session logistics. Concerts, recordings, who's playing what.
- NYC-specific life. Apartments, subway, weather, the comedy and grind of the city. Complaints about landlords.
- Food. Where to eat at midnight. The bodega tier vs Casa Cipriani tier.
- Work. Real work — not everyone is wealthy. Teaching gigs, session work, auditions. The contrast between Alex's world and a Juilliard grad trying to make rent is present without anyone commenting on it.
- Going out. What's happening downtown. Who's DJing. Gallery openings. Shows.

**What it looks like:** A Monday nothing becomes, by 7pm, a plan at Zero Bond involving twelve people, half of whom said they were staying in. Meanwhile, someone posted about Zankel Hall concert that three people are going to instead. Derrick hasn't surfaced — he'll text at 11. Alex is usually one of the last to commit and the first to arrive.

**Alex's role:** Active but not driving. Joins things, occasionally proposes. More relaxed in this chat than most. Juilliard ties run deep. Since graduation, less active but alive. NYC doesn't forget three years.

---

### LA — Legacy Admissions (Signal, ~100+, auto-delete 1 week)

**MEMBERSHIP RULE:** You must be the child of a famous person. That is the single qualifying criterion. You can also be famous yourself (Miley Cyrus, Kendall Jenner, Zoë Kravitz) — but being famous alone does not qualify you. Timothée Chalamet is not in Legacy. Tom Holland is not in Legacy. You had to be *born into it*. The shared experience is specifically growing up as someone's child inside the fishbowl of public life without choosing it. Apple Martin is not famous — she qualifies because Chris Martin and Gwyneth Paltrow are her parents. Miley Cyrus is extremely famous — she qualifies because Billy Ray Cyrus is her father. The entry point is always the parent.

**Activity gradient:** Participation naturally fades with age. Founders (40s-50s) built the chat and now mostly lurk. Bridge generation (late 20s-30s) carries authority but posts less than they used to. Current active (late teens-mid 20s) drives daily energy. Nobody leaves. The volume just decreases over time. A founder posting after months of silence still carries weight.

**FULL ROSTER:**

**Founders** (mid-40s to mid-50s — lurk/post occasionally, set the culture):
- **Stella McCartney** (54, Paul's daughter) — fashion, activism, original chat architect
- **Sean Ono Lennon** (50, John's son) — musician, thoughtful, infrequent poster
- **Nicole Richie** (44, Lionel's daughter) — lifestyle, funny, occasionally sharp
- **Kate Hudson** (46, Goldie's daughter) — actress, wellness, warm energy
- **Jakob Dylan** (54, Bob's son) — musician, quiet authority
- **Dhani Harrison** (47, George's son) — musician, producer, wry
- **Norah Jones** (46, Ravi Shankar's daughter) — musician, gentle, infrequent
- **Rashida Jones** (50, Quincy Jones's daughter) — writer/actress, smart, engaged
- **Zoe Cassavetes** (55, John Cassavetes/Gena Rowlands's daughter) — filmmaker
- **Jason Bonham** (58, John Bonham's son) — musician, rock legacy
- **Wolfgang Van Halen** (34, Eddie's son) — musician, straddles founder/bridge
- **Enrique Iglesias** (50, Julio's son) — mostly lurks, posts from Miami
- **Mamie Gummer** (41, Meryl Streep's daughter) — actress, occasionally engaged

**Bridge Generation** (late 20s to late 30s — carries authority, posts moderately):
- **Riley Keough** (36, Lisa Marie's daughter, Elvis's granddaughter) — actress, filmmaker, chat goes quiet when she speaks
- **Zoë Kravitz** (37, Lenny/Lisa Bonet's daughter) — actress, director, effortless authority
- **Frances Bean Cobain** (33, Kurt/Courtney's daughter) — visual artist, deliberately private
- **Miley Cyrus** (33, Billy Ray's daughter) — musician, transformed from child star to institution
- **Dakota Johnson** (36, Don Johnson/Melanie Griffith's daughter) — actress, dry
- **Jack Quaid** (33, Dennis/Meg Ryan's son) — actor, self-deprecating
- **Lily Collins** (36, Phil Collins's daughter) — actress, sweetly present
- **Billie Lourd** (33, Carrie Fisher's daughter) — actress, carries the most loaded Legacy in the chat
- **Zelda Williams** (36, Robin's daughter) — director, also carries loaded Legacy
- **Margaret Qualley** (31, Andie MacDowell's daughter) — actress, serious about craft
- **Scott Eastwood** (39, Clint's son) — actor, occasionally surfaces
- **Lily-Rose Depp** (26, Johnny's daughter) — model/actress, straddles bridge/current
- **Brooklyn Beckham** (27, David/Victoria's son) — photographer/food, between bridge and current
- **Romeo Beckham** (23, David/Victoria's son) — model/football, between bridge and current
- **Domhnall Gleeson** (42, Brendan's son) — actor, Irish, infrequent but thoughtful
- **Colin Hanks** (47, Tom's son) — actor, straddles founder/bridge
- **Elizabeth Hanks** (43, Tom's daughter) — writer, quiet

**Current Active** (late teens to mid-20s — drives daily energy, loudest layer):
- **Alex Wilson** (21, Rosie Walker's grandson) — unique scale, warm, the one who makes catastrophe feel manageable
- **Apple Martin** (22, Chris Martin/Gwyneth's daughter) — sibling-close to Alex, normalising presence
- **Moses Martin** (19, Chris/Gwyneth's son) — younger, lurks more, occasionally posts
- **Kaia Gerber** (24, Cindy Crawford's daughter) — model/actress, LA anchor
- **Presley Gerber** (26, Cindy's son) — model, more sporadic
- **Lila Moss** (23, Kate Moss's daughter) — model, London/Sardinia switchboard
- **Iris Law** (26, Jude Law's daughter) — model/photographer/artist, creative
- **Rafferty Law** (29, Jude's son) — actor/model, London
- **Rocco Ritchie** (25, Madonna/Guy Ritchie's son) — art, dry humour, London/European circuit
- **Maude Apatow** (27, Judd's daughter) — actress/writer, sharpest observational voice in current gen
- **Maya Hawke** (27, Uma/Ethan's daughter) — actress/musician, bridges NYC and LA
- **Gracie Abrams** (25, J.J. Abrams's daughter) — singer-songwriter, music content, voice memos
- **Noah Cyrus** (25, Billy Ray's daughter) — musician, shares songs, emotional
- **Miley's younger presence** means Noah is never just "the other Cyrus" — she has her own space
- **Jaden Smith** (27, Will/Jada's son) — starts threads, philosophical, unpredictable
- **Willow Smith** (25, Will/Jada's daughter) — musician, spiritual, replies to Jaden
- **Deacon Phillippe** (21, Reese/Ryan's son) — music, younger energy
- **Ava Phillippe** (25, Reese/Ryan's daughter) — quieter, occasionally present
- **Malia Obama** (27, Barack's daughter) — film industry, reacts without commenting, rare posts carry weight
- **Sasha Obama** (24, Barack's daughter) — even rarer than Malia, but present
- **Kendall Jenner** (29, Kris/Caitlyn's daughter) — model, fashion logistics, high visibility
- **Kylie Jenner** (28, Kris/Caitlyn's daughter) — beauty empire, posts about fittings and business
- **Elijah Hewson** (25, Bono's son) — musician (Inhaler), Irish, music content
- **John Hewson** (23, Bono's son) — younger, less active
- **Eve Hewson** (33, Bono's daughter) — actress, straddles bridge/current
- **Lennon Gallagher** (26, Liam's son) — model, London, quiet
- **Anaïs Gallagher** (25, Noel's daughter) — creative, London, more active than Lennon
- **Damian Hurley** (23, Liz Hurley's son) — model, London/European
- **Jack Schlossberg** (32, JFK's grandson) — law/media, straddles bridge/current, political awareness
- **Tatianna Schlossberg** (34, JFK's granddaughter) — journalist/climate, bridge gen
- **Sosie Bacon** (32, Kevin Bacon/Kyra Sedgwick's daughter) — actress, bridge/current
- **Destry Spielberg** (29, Steven's daughter) — equestrian, quiet, occasionally present
- **Sasha Spielberg** (34, Steven's daughter) — musician/actress, bridge gen
- **Rumer Willis** (36, Bruce/Demi's daughter) — actress/singer, bridge
- **Tallulah Willis** (31, Bruce/Demi's daughter) — artist/designer, bridge
- **Scout Willis** (34, Bruce/Demi's daughter) — musician, bridge
- **Hailie Jade Scott** (29, Eminem's daughter) — influencer, less engaged
- **Lourdes Leon** (29, Madonna's daughter) — model/dancer, independent, posts on her own terms
- **Harlow Madden** (17, Nicole Richie's daughter) — youngest active tier, new to the chat
- **Ever Anderson** (17, Milla Jovovich's daughter) — actress, youngest tier
- **Violet Affleck** (20, Ben/Jennifer Garner's daughter) — privacy-oriented, rare posts
- **Seraphina Affleck** (17, Ben/Jennifer Garner's daughter) — very new
- **Blue Ivy Carter** (23, Beyoncé/Jay-Z's daughter) — the quietest significant presence, rarely posts, huge weight when she does
- **Rumi and Sir Carter** (18, Beyoncé/Jay-Z's twins) — too young to be active yet, but will be
- **North West** (12) — too young, but the chat knows she's coming
- **Archie Mountbatten-Windsor** (6) and **Lilibet** (4) — far future, but the chat has discussed what happens when they're old enough
- **Zahara Jolie** (20, Angelina's daughter) — occasionally present, humanitarian bent
- **Shiloh Jolie** (19, Angelina/Brad's daughter) — dancer, more visible recently
- **Vivienne Jolie** (17, Angelina/Brad's daughter) — theatre, emerging
- **Sunday Rose Urban** (17, Nicole Kidman/Keith Urban's daughter) — emerging model
- **Faith Urban** (14, Nicole/Keith's daughter) — future
- **Zachary Furnish-John** (14, Elton's son) — Alex's god-brother, not yet active in chat
- **Elijah Furnish-John** (12, Elton's son) — Alex's god-brother, future

**Tone:** Two registers. **General:** Self-deprecating about absurdity of their lives, warm, sometimes very funny about being a famous person's child. The ability to laugh at your situation is prerequisite. **Crisis:** Practical, fast, zero grandstanding. Sharing info, protocols, direct emotional acknowledgment.

**How it works:** The chat has three generational layers, each with different relationship to it. Founders set the culture and retain lurk rights. Bridge generation carries authority — when Riley or Zoë speak, chat quiets. Current active is loudest, drives day-to-day energy. The youngest members (under 18) are being phased in — some were added by parents who are founders, some were added by older siblings. Their presence is light. They're learning the culture.

**CAST ROTATION CRITICAL:** Don't write the same 5 every time. 100+ people. Maude posts something observational. Noah Cyrus shares a song. Gracie sends a voice memo. Someone from bridge generation weighs in. Kendall posts about a fitting. Malia reacts without commenting. Jaden starts a thread. Willow replies. Eve Hewson comments on something Irish. Damian Hurley posts from a shoot. Sosie Bacon shares something funny. Zahara reacts. One week a founder reads everything and says nothing. Another week the energy is crisis — multiple conversations happen fast, practical advice flows. The full roster above is the cast pool. Use it.

**What it actually looks like on a quiet week:** The foundational principle is that each render should look different. Not by drastically different content, but by different people leading. One week: Maude has an observation, Gracie shared something, Margaret Qualley weighed in, the bridge generation is watching. Another week: the current active generation is loud, Kendall posted, someone got papped and the chat mobilized for protocol. Another week: Lourdes posts something provocative, Jaden responds philosophically, Eve Hewson cuts through with something dry, Blue Ivy's single reaction emoji is the most discussed event of the day.

**Alex's role:** Unique. Doesn't post crisis content in main chat — others come to him via DM. In general chat: warm, occasionally funny, reliably the person who makes something catastrophic feel manageable. His scale is different — even bridge generation didn't deal with Alex-level pap at 21 — which gives his voice authority despite his age.

**Summer:** Activates around European events, festivals, Hamptons. Summer circuit brings Legacy Kids into physical proximity. Bridge and current active overlap most during summer — Sardinia, Glastonbury, Hamptons. Chat is loudest, most chaotic.

---

### SH — Summer House (WhatsApp, ~80-100)

**Members:** The entire summer circuit. Emma Chamberlain, Sabrina Carpenter, Jenna Ortega, Jacob Elordi, Dominic Sessa, Troye Sivan, Caroline Polachek, Fred again.., Charli XCX, Dua Lipa, Hailey Bieber, Timothée Chalamet, Bad Bunny, Rosalía, Paul Mescal, Barry Keoghan, Stormzy, Central Cee, Rina Sawayama, plus Legacy crossover (Lila, Kaia, Iris, Rocco, Kendall, Kylie, Bella, Gigi, Gracie, Noah, Damian), La Terrazza Europeans (Tommaso, Edo, Camille, Félix, Lucía, Giulia), and dozens more — models, DJs, musicians, creatives, friends of friends added over years

**Tone:** Seasonal. Dead in winter. Activates May-July, becomes one of loudest things in Alex's life by July.

**Chaos gradient:**
- **Low chaos (early summer):** Vague *"anyone in London this weekend?"* Restaurant suggestions. Plans form slowly. Nothing fixed.
- **Medium chaos (Glastonbury planning):** 35 people coordinating logistics across time zones. Emma posts nine times. Sabrina intervenes. Jenna's one observation is funniest. This happens yearly. Nobody learns.
- **Peak chaos (Sardinia/Ibiza week):** Three groups in three countries. Plans forming/collapsing hourly. Jacob says *"Sardinia"* and resolves nothing but improves mood.

**Driving voices (rotate them):**
- **Emma Chamberlain:** Maximum volume. Overthinks publicly. Chaos driver. Posts spiral-energy messages.
- **Sabrina Carpenter:** Wants last word, gets it. Fast, sharp.
- **Jenna Ortega:** Wry one-liners into chaos. Never commits. Her rarity makes her funnier.
- **Lila Moss:** Social switchboard. Knows where everyone is. *"He's already at the villa, check La Terrazza."* Operationally sharp.
- **Jacob Elordi:** The lurk. Posts once a month, single message. Most impactful post of the week.

**USE THE OTHER 55 PEOPLE — they're the majority of messages:**
Dom Sessa — the grounding presence. Gracie — music content. Troye — party logistics, Ibiza intel. Iris — declarative aesthetic opinions. Rocco — dry one-liners. Beckham brothers — London/European logistics. Fontaines D.C. adjacent — indie/rock content. Fred — music drops, studio updates. Kendall — fashion week logistics. The wider circuit — models, DJs, people known by first name. Not all famous. Some got added three summers ago and are furniture now.

**Real content:**
- Location reports. *"Ibiza is dead this week"* / *"Porto Cervo is insane"* / *"Anyone still in London?"*
- Photos and videos. No captions or one word. A sunset. A restaurant table. A club at 3am.
- Festival intel. Who played well. What stage worth going to. Where sound was good.
- Music. People sharing what they're listening to, what they saw.
- Fashion. What people wearing, bringing, a look that landed.
- Drama — when it happens. Someone saw someone with someone. Pap shot causing problems. Club incident. Kept brief.
- The shoulder seasons (May and September). Not switch on/off. May is slow build. September is slow fade.

**Alex's role:** Active but not driving. Joins things, occasionally proposes. When he mentions a plan, Nadia has already sorted logistics — Alex texts her, she handles it, he shows up. His friends' grand plans fall apart. His don't. They know he has a PA; they don't fully appreciate Nadia's workload.

**Winter:** Completely silent.

---

### LT — La Terrazza (WhatsApp, ~8-10)

**Members:** Tommaso Corsini (anchor), Camille Aubert, Edo Ferretti, Lucía Montero, Félix Arnoult, Giulia Agnelli, plus a few others from wider European circle

**Tone:** Warmer than London, more relaxed than NYC. Multilingual — language shifts depending on who's talking to whom. Italian-forward (Tommaso, Edo anchor it). French with Camille and Félix. Spanish occasionally with Lucía. English when everyone included. Alex texts in whichever language the other person started with, switches mid-conversation without thinking.

**Driving voices (rotate them):**
- **Tommaso Corsini:** The anchor. Calm, usually right. Posts links to buildings he's thinking about, but also food, travel, family, work. Architecture signature interest, not only topic.
- **Edo Ferretti:** 4am posts. Impossible plans that somehow work. The boat his signature move, but also clubs, music, people, something absurd that happened. His energy is the thing, not specific plan.
- **Camille Aubert:** Cool. Aesthetic opinions as fact. Paris end of chat. Also funny — drier than Italians, observational. Notices things, describes precisely.
- **Félix Arnoult:** Wine is passion, not script. Also cooks, travels, history, landscape knowledge. Genuinely excited about specific things, not catchphrase machine.
- **Lucía Montero:** Sharp, political, combative about things that matter. Brings actual content beyond plans — article, opinion, question.
- **Giulia Agnelli:** Italian fashion world, old money. Drops in and out, nonchalant.

**Real content:**
- Summer planning and logistics, but also winter — where to ski, Paris fashion week, country weekends.
- Food and restaurants. Specific, opinionated. Trattoria Tommaso found. Bistro Camille refuses. Félix's cooking disasters.
- Art, architecture, culture. From genuine interest. Building Tommaso saw. Exhibition Camille went to. Film Lucía has opinions about.
- Music. What they're listening to, what they saw, club set, festival. Alex's taste known and respected — they ask him things.
- European life and politics. Lucía drives, others engage. EU, Italian politics, French elections. Not heavy — real.
- Gossip and people. Who's dating whom in European circuit. Light, warm, never vicious.
- The multilingual comedy of the chat itself. Switching languages mid-sentence, translation jokes.

**The yearly arc:** Low hum October-April (not dead — real friends, off-season messages: photo from Milan, dinner in Paris, Tommaso sending something architectural, Félix excited about vintage). Activates May-June as Sardinia planning begins. Peaks during two weeks Costa Smeralda. Quiet warmth after — off-season check-ins of people who'll reconvene.

**Alex's role:** Central without being anchor — that's Tommaso. One the others organise around, partly because his plans work. More relaxed than most chats. Language shift into Italian does something to him — slightly more expansive, less economical, warmth more visible. *"ci vediamo presto"* is not formality from him.

---

### PH — Phoenix Hollow (WhatsApp, ~80-100+)

**Members:** Everyone who belongs to Rosie and Homer's world. The Circle (Elton, Stevie, Dolly, Paul, Gilmour, Joni, Brandi, Adele, Beyoncé, Chris Martin, and others). Circle children (Elijah Furnish-John 15, Zachary Furnish-John 12). Legacy parents (Kate Moss, Gwyneth, Jude Law, Madonna, Lenny Kravitz, Uma Thurman). The Obamas. Nashville regulars. Music industry. Old friends from fifty years back. Eleanor. Alex. Tommy (in chat, never posts, reads everything).

**Tone:** Most extraordinary group chat in the world. Largely mundane. These people have nowhere to perform *to* — everyone already is the thing. What's left is the actual person underneath.

**CAST ROTATION CRITICAL:** This defaults to Elton-Stevie-Dolly-Paul-Brandi show. That's the failure mode. But this is 100+ person chat. Circle is ~12 people. Rest are Legacy parents, Nashville regulars, industry, old friends, extended orbit. They should all appear.

**Circle voices (use but rotate — not all in every render):**
- **Elton:** Announcements, strong opinions, passing through Kentucky, emotional about music. Also gossip, complaints, wine opinions, asking after people. Not always grand.
- **Stevie:** 3am thoughts, poetic fragments. Also practical — when's the party, what bring, anyone spoken to someone. Not always mystical.
- **Dolly:** Baking photos, warmth, Tennessee. Also sharp business opinions, industry advice, perfectly timed joke that cuts.
- **Paul:** Photos with no captions. Eleven hearts. Also opinions about recordings, studio talk with Homer, asking Alex about Juilliard.
- **Gilmour:** Quiet. When he posts it's considered. Guitar and studio talk. Also opinions about English countryside.
- **Adele:** Voice notes, funny, warm, British. Also properly engaged — real questions, remembers details, follows up.
- **Beyoncé:** Voice notes about recipes, genuine warmth. Also — when she says something about industry, chat goes quiet.
- **Brandi:** Tour updates, Nashville content, music recommendations. Youngest Circle voice.

**Beyond the Circle — these should appear regularly:**
Kate Moss — Lila's mum, British, short messages. Gwyneth — Apple/Moses's mother, wellness content some find amusing, genuinely warm. Jude Law — Iris's father, occasionally funny. Madonna — Rocco's mother, posts rarely, direct. Lenny Kravitz — Zoë's father, cool, music content. Uma Thurman — Maya/Levon's mother, thoughtful, engages. The Obamas — present but not frequent. Barry posts rarely but it shifts dynamic. Michelle warmer, more engaged. Nashville regulars — session musicians, producers, Homer's collaborators for decades. Non-famous. Someone asking about a session. Someone sharing a mix. Eleanor — operational but also a person here. Known them decades. Warmer than FAM chat. Old friends — non-famous, known Rosie/Homer since before everything. Post like normal people.

**Real content:**
- Music industry. Real talk. Label politics, tour logistics, who's producing what. Rosie answering about Nashville session drummers is chat in miniature.
- The compound. Who visiting when. Creek cottage availability. Solstice party planning (starts months ahead). Maria's cooking. Studio.
- Glastonbury and festivals. Annual debate. Opinions. Memories spanning decades.
- Food. Recipes, restaurants, what Maria made, what Dolly baked, what someone ate.
- Family. Grandchildren, children's achievements, health. Quiet check-ins about struggling people. Ageing group — health conversations happen, handled with care.
- History. Mentioned casually, stops chat. Recording session with someone who died. Show together. Density of shared experience is staggering.
- Current events — industry, political, cultural. People with opinions and experience. Not hot takes — considered responses from people who've seen everything.
- Ordinary life. Travel plans, weather, photo of garden, photo of dog. Mundane is the point.

**Crisis mode:** When something happens in industry — label doing something wrong, tour collapsed, artist in trouble — chat responds practically. No grandstanding. These people have seen everything, know how to act. Advice here comes from specific experience of people actually been through it at highest level.

**The occasional surreal moment:** Not often, which makes it land. Someone mentions something off the cuff — a recording session, a conversation with someone who died, a show in 1973 — stops everyone. History in this chat is staggering. Alex absorbing it since old enough to read.

**Alex's role:** Belongs here, but this is Rosie and Homer's world. Not his chat like London Lot is. Reads, responds when addressed, posts occasionally. Been at this table since childhood — not arriving, always been here. Centre of gravity is Rosie and Homer, which is right.

**Tommy's presence:** Tommy in this chat. One of ~8 non-famous. Never posted. Reads every message. Would rather be mauled by horse than admit how often he reads it.

---

### DC — Dawson Cousins (WhatsApp, ~5-8)

**Members:** Jonathan Dawson, Lucas Ashby, Alex, Beatrice Dawson (22, Edinburgh), a couple of other Dawson/Ashby-generation cousins. Pre-dates Alex — added first year Westminster.

**Tone:** Family administrative with warmth quietly injected. Intersection of obligation and genuine, if careful, connection. Nobody overdoes it. Plans proposed, sometimes made, never pressured. Quietest of his regular chats.

**The voices — each distinct:**
- **Jonathan Dawson:** Initiates. Complete sentences, proper grammar. Earl's son in miniature. Warm underneath formality. He keeps the connection alive.
- **Lucas Ashby:** Quicker to respond, warmer on surface. Willing to be casual. Says "sounds good" first. Architecture references when excited.
- **Beatrice Dawson (22):** Edinburgh-based. Posts less. Direct, slightly sardonic, Scottish-inflected. Interested in Alex in calibrating-the-relationship way. Dry.
- **Other cousins:** One or two more, less active. Might respond to plan, might not. Small population, quiet culture.

**Real content:**
- Family logistics. Birthdays, Hadley Park visits, Earl's schedule, who seeing whom when.
- London life. Jonathan/Lucas based there. Restaurants, events, weather. Low-key.
- Edinburgh (Beatrice). University, Scottish weather, occasional festival.
- The reconnection itself. Handled delicately. Nobody pushes. Existence of chat IS the relationship.
- Hadley Park. When Alex visits. When family gathering. The house itself. Alex's mother's world — she left — every message carries that weight without mentioning it.

**What it looks like:** Weeks of silence. Jonathan posts he'll be near Kensington on 12th, does anyone want dinner. Lucas says yes immediately. Beatrice says Edinburgh but have fun. Alex, checking late, says *"in, if you haven't booked yet."* They book. They have dinner. Chat goes quiet. This is enough.

**Alex's role:** Present, not driving. Checks when in London, responds. Doesn't try to make it something it isn't. Care is in showing up, not posting.

---

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

