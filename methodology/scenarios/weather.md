# Weather scenarios

=== scenario 127 | weather | D | s | corpus ===
scenario: weather small talk with an elderly neighbor
zones: weather,comparative,tags-backchannel
intent: A younger neighbor and an elderly neighbor trade small talk about the weather, comparing it to other days.
beats:
- the younger neighbor opens with a remark on the weather
- the elderly neighbor agrees and compares it to a day earlier in the week
- a backchannel murmur keeps the exchange moving
- the elderly neighbor tops it with a memory of a similar stretch from years back
- they part on a guess about what tomorrow will bring
held:
- the weather that day, named plainly (hot, cold, wet, or still)
- the day earlier in the week it gets compared to
- the elderly neighbor's remembered stretch, from a stated number of years back
- the guess about the next day
cast: a younger neighbor; an elderly neighbor; they label their own turns however such neighbors would address each other.
text: A younger neighbor runs into an elderly one outside and opens with a remark on the weather that day. The elderly neighbor agrees, comparing it to a day earlier in the week, and the younger one murmurs along in agreement. The elderly neighbor tops it with a memory of a similar stretch from years back, told plainly, not as a lesson. They label their own turns however such neighbors would address each other. Write the exchange, ending with a guess between them about what tomorrow will bring.
=== end ===

=== scenario 128 | weather | M | l | corpus ===
scenario: the storm as it came in and what it took
zones: past-narrative,weather,exclamation
intent: Someone tells the whole story of a storm, from the first sign of it to everything it ended up taking.
beats:
- the stillness and the look of the sky before the storm broke
- the first warning, wind picking up within the hour
- rushing outside to secure what could still be tied down or brought in
- the household gathering close together as the wind kept rising
- the power going out
- the worst of it, the wind loud enough that talking stopped
- a tree coming down close enough to hear it land
- part of the roof stripped away
- a window that cracked but held
- the fear during the worst stretch, admitted only afterward
- the sudden quiet when it finally passed
- stepping outside to survey what was left
- the tree found blocking the way out until it could be cleared
- the tally taken afterward: the roof, the tree, a neighbor's fence gone entirely, and the days of cleanup that followed
held:
- the wind picked up within the hour of the sky going still
- the household gathered close together once the wind kept rising
- the power went out during the worst of it and stayed out for two days
- one tree came down close enough to hear it land
- part of the roof was stripped away
- a window cracked but held
- the worst stretch lasted under half an hour, the loudest anyone there had heard
- the tree ended up blocking the way out until it was cleared
- a neighbor's fence was flattened entirely
- cleanup ran the better part of a week
cast: the one telling it, who lived through the storm; the household with them, kin; whoever hears the telling stays out of scene.
text: A storm rolled in on you and your household, and you are telling the whole story of it now, start to finish. The sky had gone still and strange before it broke, and within the hour the wind was picking up enough to send you rushing outside to tie down or bring in whatever could still be moved. By the time the wind was really rising you had everyone gathered close together, and the power went out not long after. Tell the worst of it: the wind loud enough that talking stopped, a tree coming down close enough to hear it land, part of the roof stripped away, one window that cracked but held, and the fear you only admitted to afterward. Tell the sudden quiet when it finally passed, and stepping outside to see what was left: the tree blocking the way out until it could be cleared, the roof needing real repair, and a neighbor's fence flattened entirely by comparison to what you lost. Close with the days of cleanup that followed and how you tell it now, still reaching for the exclamations when you get to the worst parts.
=== end ===

=== scenario 129 | weather | M | m | corpus ===
scenario: the fire nearby: watched, fled, recounted
zones: past-narrative,weather,body
intent: Someone recounts watching a fire spread nearby, the decision to flee, and how it felt in the body while leaving.
beats:
- smoke first noticed on the horizon in the early afternoon
- checking again within the hour, the smoke thicker and the wind pushing it closer
- the decision point, watching turning to leaving once the smoke stung the eyes
- grabbing only what mattered and being out within a short stretch
- the throat going raw and the heat felt on the skin while leaving
- glancing back at the light of it while getting clear
- the wait, gone two nights, not knowing
- the return, finding the place spared
held:
- smoke first seen in the early afternoon, still distant
- within the hour, the wind had pushed it close enough to sting the eyes
- out of the place within twenty minutes of deciding to go
- the throat left raw and the heat felt on exposed skin while leaving
- gone two nights before being allowed back
- the place found standing, spared, on return
cast: the one telling it, who watched and then fled; the household with them; whoever hears the telling stays out of scene.
text: You watched a fire spreading nearby before you fled it, and you are recounting the whole thing now. Tell how the smoke first showed on the horizon in the early afternoon, still distant enough to just watch; how within the hour the wind had pushed it close enough that the smoke started to sting your eyes; and the moment watching turned into leaving. Tell how fast you moved once you decided, out of the place within twenty minutes with only what mattered; how your throat went raw and the heat pressed against your skin on the way out; and the glance back at the light of it as you got clear. Tell the two nights you spent away not knowing, and finally getting to go back and finding the place had been spared.
=== end ===

=== scenario 130 | weather | M | m | control ===
scenario: the rising water: the flood, hour by hour
zones: temporal,weather,numbers
intent: Someone recounts a flood's rise hour by hour, from the first water at the door to the water finally going down.
beats:
- the water first noticed at the door in the early morning, ankle deep
- checked again an hour later, already higher
- moving things up off the floor while there was still time
- reaching knee height by midmorning, everything moved onto whatever in the place stood highest
- the water still climbing into early afternoon
- peaking in early afternoon, past the highest point anything had been raised to
- the wait through the worst of it, listening to it against the walls
- the water starting to recede several hours after the peak, and going back the next day to see the line it left
held:
- first noticed at the door in the early morning, ankle deep
- an hour later noticeably higher
- reached knee height by midmorning, everything moved onto whatever stood highest in the place
- peaked in early afternoon, past the highest point anything had been raised to
- began receding several hours after the peak
- gone by the next day, leaving a mark on the walls
cast: the one telling it, who watched the water rise; the household with them; whoever hears the telling stays out of scene.
text: A flood rose through your place and you are telling it hour by hour, the way you lived it. Start with the water first at the door in the early morning, only ankle deep; checked again an hour later and already higher, enough that you started moving things up off the floor while there was still time. Tell how by midmorning it had reached knee height and you moved everything you could onto whatever stood highest, and how it kept climbing until it peaked in early afternoon, past the highest point anything had been raised to. Tell the wait through the worst of it, listening to the water against the walls, and how, several hours after the peak, it finally started to go down. Close with going back the next day to see the line it left behind on the walls.
=== end ===

=== scenario 131 | weather | D | s | control ===
scenario: the rain that broke the dry spell, celebrated
zones: weather,exclamation,intensifier
intent: A household celebrates the first rain that finally breaks a long dry spell.
beats:
- the first drops noticed and called out
- everyone rushing to the window or outside
- an exclamation over how badly it was needed
- someone exaggerating the celebration, half joking
- settling to just stand and listen to it fall
held:
- the dry spell had run for a stated number of weeks
- the first drop noticed at a stated moment, just after midday
- the exclamation naming how badly it was needed
- how long they stood outside just listening to it
cast: a household, however many are home; they label their own turns however such people would call each other.
text: A household has been waiting out a dry spell that has run for weeks, and the first drops finally fall just after midday. One of them calls it out, and everyone rushes to the window or straight outside. There is an exclamation over how badly it was needed, and someone exaggerates the celebration, half joking, arms out to it. They label their own turns however such people would call each other. Write the exchange, ending with them standing outside just listening to it fall.
=== end ===

=== scenario 132 | weather | M | m | corpus ===
scenario: the hardest cold anyone remembers
zones: comparative,weather,past-narrative
intent: Someone recounts the hardest cold spell anyone in the household remembers, measured against past winters.
beats:
- the cold setting in, colder than expected from the first day
- it holding without breaking for eleven days straight
- the coping measure taken, kept up around the clock
- something outside failing because of the cold that doesn't normally
- the oldest one present comparing it to a spell from decades back
- the single worst night, pinned as the coldest point
- what was lost to the cold
- the eventual thaw, when it finally let up
held:
- held hard for eleven days straight without a break
- a fire or stove kept going around the clock as the coping measure
- something froze that never had before, a water source or a pipe
- the oldest one present compares it to a spell from decades back
- the single coldest night marked as the worst of the stretch
- a crop or an animal lost to the cold
- the thaw finally came after the eleven days
cast: the one telling it; the oldest one present, giving the comparison; the household, kin; whoever hears the telling stays out of scene.
text: The hardest cold anyone in your household can remember set in and held for eleven days straight without a break, and you are telling the whole stretch of it now. Tell how it was colder than expected from the very first day, and how you kept a fire or stove going around the clock just to manage. Tell what failed because of it that never had before, a water source or a pipe freezing solid. Tell how the oldest one in the house set it against a cold spell from decades back and said this one beat it. Mark the single worst night as the coldest point of the whole stretch, and what the cold ended up costing you, a crop or an animal lost to it. Close with the thaw finally coming after those eleven days, and what it felt like when it broke.
=== end ===

=== scenario 133 | weather | M | l | corpus ===
scenario: the year in the garden plot: wins, pests, politics
zones: past-narrative,temporal,food
intent: Someone tells the whole year in their garden plot, the wins, the pests, and the small politics with the other growers, start to finish.
beats:
- deciding what to plant, settled in early spring
- planting a few weeks after the last cold
- a run of good weather that got everything off to a strong start
- the first pest turning up on one crop
- the remedy tried, working only partly
- a dry stretch partway through the season
- hauling water by hand daily to get through it
- a dispute with a neighboring plot-holder over a shared water turn
- the dispute finally getting settled between them
- the best-producing crop of the year, a clear win
- a second problem, birds or rot, hitting a different crop
- a storm partway through the season flattening several rows
- the work of pulling the rows back up afterward
- the harvest finally tallied at the end
- some of it traded to another grower for something needed more
- the plot put to bed for winter, and your verdict on the year, looking back
held:
- planted a few weeks after the last cold, in early spring
- the first pest identified on a stated crop
- the remedy tried worked only partly
- the dry stretch had water hauled by hand daily for weeks
- the dispute with the neighboring plot-holder was over a shared water turn
- the best crop of the year, named, and its count
- a storm partway through flattened several rows
- the harvest tallied at the end, a stated total
- some of the harvest traded to another grower for something needed more
- the plot closed up for winter at the end
cast: the one telling it, tending their own plot; the neighboring plot-holder in the dispute; the other growers on the shared ground; whoever hears the telling stays out of scene.
text: You kept a garden plot this past year and you are telling the whole year of it, start to finish: the wins, the pests, and the small politics with the other growers. Tell how you settled on what to plant in early spring and put it in a few weeks after the last cold, and how a run of good weather got everything off to a strong start. Tell the first pest that turned up on one of the crops, the remedy you tried that only partly worked, and the dry stretch partway through the season that had you hauling water by hand daily for weeks just to keep things alive. Tell the dispute that grew out of it with a neighboring plot-holder over whose turn it was for the water, and how that finally got settled between you. Tell your best-producing crop of the year, a clear win by any measure, set against the second problem, birds or rot, that hit a different crop instead. Tell the storm partway through that flattened several rows and the work of pulling them back up afterward. Close with the harvest finally tallied at the end, some of it traded to another grower for something you needed more, and the plot put to bed for winter, and give your own verdict looking back on the whole year of it.
=== end ===

=== scenario 134 | weather | M | m | control ===
scenario: the best harvest anyone remembers
zones: comparative,past-narrative,numbers
intent: Someone recounts the best harvest anyone can remember, set against past years by the numbers.
beats:
- the harvest coming in far beyond what was expected, noticed early
- one crop specifically doing far better than usual, a stated multiple
- compared against the previous best, from a stated number of years back
- extra hands, a stated number, brought in to help bring it all in
- what was done with the surplus once the usual need was covered
- the oldest grower present giving the comparison against their whole memory
- what got credited for the good year
- how it is still talked about now
held:
- came in at nearly twice the usual amount
- one crop stood out, its count stated plainly
- the previous best was a stated number of years back
- extra hands were brought in to help
- the surplus went to storage and to trade once the usual need was covered
- the oldest grower present set it against their whole memory and called it the best
- credited to rain arriving at the right time and a mild stretch through the season
cast: the one telling it, who worked the harvest; the oldest grower present, giving the comparison; the other hands who helped; whoever hears the telling stays out of scene.
text: The best harvest anyone can remember came in this year, and you are telling the whole story of it, set against the numbers from past years. Tell how it was clear early that this one would beat the rest, coming in at nearly twice the usual amount. Tell the one crop that stood out above everything else, its count far past what it usually gives, and set it against the previous best, from years back. Tell how extra hands had to be brought in just to get it all in before it turned, and what was done with the surplus once the usual need was covered, some stored, some traded on. Tell how the oldest grower present set this year against their whole memory and called it the best they had seen, and what got credited for it, rain arriving at the right time and a mild stretch through the season. Close with how it is still talked about now, the year everyone measures the others against.
=== end ===
