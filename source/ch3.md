# Chapter 3: The Camera

Synopsis: Much like the RTS games that inspired it, the dota genre is most commonly played with a top-down "free roaming" camera that can be moved around the map independently of the participants. The genre features many mechanics that take advantage of the free camera and most dota players favor the free camera. However, the RTS genre was designed for a world in which you are playing the role of an overhead commander, whereas dota asks you to play the role of an individual. The use of a free camera to control an individual breaks the player's connection to the action on the screen and does it to a substantial detriment. This faulty design choice is countered by an excellent body of game design that shows it is possible to manage RTS elements from a fixed camera perspective. But ultimately, the resistance of the dota community to fixed camera elements has nothing to do with an argument of superiority. Quite simply, it is a fear of change, a fear that a fixed camera would "dumb down" the genre. It is a fear generated by a lack of familiarity with the games that have featured the fixed camera elements and done them well.

---

The two most fundamental design choices you will make in the creation of your game are input and output. How will players control the events in the world and how will they view them? If your game is worth a damn, then these decisions will profoundly govern its design. Throughout videogame history, game developers have had significant agency to shape these choices. Very often, the people creating the games were also creating the hardware.[^1] But it's not just hardware that can dictate input and output. This can also happen at the software level, where an existing game engine or game creation software dictates the range of design choices. These lessons are most obvious in any discussion of the dota genre's approach to output.

Aeon of Strife and Defense of the Ancients employ the common real-time strategy camera system, a top-down "free-roaming" camera conceived in the strategy games prior to StarCraft and Warcraft III. In these games, the camera has a limited field of view and does not follow any one target. Instead, the player manages the location of the camera just as they would manage the location of their character or their soldiers. While games such as Awesomenauts, Smite, Dead Island: Epidemic, and console dota games are designed for a fixed camera—where the camera locks directly to the character you have chosen for battle—this is not the standard option. The most popular philosophy sticks with the roots, and games such as League of Legends, Dota 2, Dawngate, Demigod, Heroes of the Storm, and a rash of Chinese dota knockoffs favor the free camera. These games typically offer a toggle between the free and fixed methods, but the fixed camera is typically a concession to beginners who are uncomfortable with managing the camera as a separate entity. This is because Defense of the Ancients and subsequent dota games feature game systems and game mechanics which have been designed for use with the free camera.

Dota is a genre where it is crucial for teammates to hit lanes and angles simultaneously in order to synchronize skills into a well-coordinated path of destruction. In the pursuit of proper timing, players expect a grasp of the battlefield that cannot always be conveyed through an on-screen minimap or player communication. It's easier for those players to move the camera around the battlefield and see where teammates and enemies are coming from. But in addition, many dota games feature elements familiar to RTS games, and the free camera is designed to take advantage of them. In many dota games, the player can acquire a courier, which will allow players to purchase items from the shopkeepers in their base and transport the items to their character while they are in the battlefield. Management of the vulnerable courier as it moves through the winding battlefield is very often a must. On top of this, many characters can either create clones of themselves or summon supporting units. Since they can be managed as individual entities, they can be used to attack and defend multiple fronts.

Because dota has been designed for the free camera, comprehension and mastery of the camera are mandatory for "skilled play" in the games which provide it. And when confronted with the option of designing a dota game for a free camera or a fixed camera, the free camera is usually the one that wins out. However, it will be a common theme in this book that simply polishing, tailoring, or adapting your game systems for an idea does not act as good game design unto itself. If you have a good eye for movies or television, you know that merely tying together the loose ends does not make a conclusion fulfilling. An ending can still be a bad one even if "It makes sense, given the options they had to work with." It is about deriving an interesting end result from the sum of all parts.

So, we need to understand two things: Why did the dota genre adopt the free camera and what is the actual purpose of a free camera? The first question is pretty easy to answer. The dota genre uses the free camera because Warcraft III did. (That will also be a common theme in this book.) But if you are familiar with Warcraft III mapmaking, then you are aware the camera is one of the few things that mapmakers actually had full control of. You can zoom, rotate, and position the camera in any way that you want. You can even build your game map for fixed camera support, locking the camera to a character from a third-person or first-person viewpoint. Map creators had a fairly wide range of choices to work with, so what happened here?

Well, Battle.net custom maps were foremost a social affair, and the maps were usually designed for the highest player counts possible. Much in the way that today's big-budget videogames are often homogenized so that they will be agreeable to large audiences, the high player counts effectively democratized the decision to continue playing a map. If ten players get together to play a map and only one of them does not like the concept, the control scheme, or even a specific aspect of the map, then that's ten people who may move on to a different map.

If your goal was to make a popular Warcraft III custom map, you didn't risk the trend that an unconventional concept would take some time to become comfortable with, even if it's an interesting one. The creators that took the Warcraft III game engine in unconventional directions watched their projects become niche affairs, closer to proof-of-concept than a mainstay in the Warcraft III custom game listings. And within the context of an RTS game with a free camera, and in a game where the company's art assets and game mechanics were tailored towards a very specific field of view, a camera that locks to a character amounts to a gimmick.[^2] This is where the problem lies. The Warcraft III game engine has so thoroughly dictated output in the dota genre that the field of view in the games that use the free camera is almost entirely identical. And, in using this free camera, the dota genre has entirely compromised the way that you view and connect with that virtual universe.

In using a free camera as the backbone for the dota genre, designers and developers have completely missed the point as to why RTS games use a free camera. It has nothing to do with "giving players the tools they need to win". When you play a videogame, ask yourself a simple question: Who are you playing as? That is the most fundamental means by which you connect with the action on the screen, by inserting yourself in the role of some participant in that world.[^3] There is no mincing words when we describe this as fundamental to the character of a videogame. Whether maze games, platformers, shoot 'em ups, side-scrolling action games, fighting games, 2D and 3D brawlers, adventure games, stealth games, or even work and flight simulators, all of these games use some variant of a fixed camera.[^4] Even games which employ multiple characters—particularly team-based fighting games—make sure to keep your current character in the field of play or quickly shift the camera to the next participant in order to maintain the player's connection to the action.

The RTS camera was designed for a world in which you are playing as a commander, and you are looking down on the universe you are helping to shape.[^5] The genre and its pioneers had already figured this out in their early years, where Dune II: The Building of a Dynasty placed you directly in a generic leading role and Populous asserted that you were a god looking down on your followers. Even in the RTS games which do not provide a direct narrative context for your role in the game, the game model conveys the commander role. So even if Supreme Commander and Total Annihilation thrust "you" directly onto the battlefield as a king-style chess piece,[^6] and The Lord of the Rings: Battle For Middle-Earth places you in the unspoken role of the narrator, the focus is on managing the simulation of war and making sure your soldiers go where they need to go. It's not only empowering to scan the battlefield and give orders, but it feels comfortable and natural.

The dota genre has adopted the RTS commander role for use in a game where you are centrally playing as one character. You are not playing as the courier, you are not playing as your summoned creatures, you are not playing as your supporting soldiers, and you are not playing as the collective of those moving parts. You are playing the character you have chosen for battle, so it is natural that the action is always focused on "you" or from "your perspective".[^7] Through the use of the free camera, you are constantly detaching yourself from the character that is supposed to be your connection to the action on the screen. Immersion is the popular buzzword these days, and let's be very clear: This breaks immersion and does it to a substantial detriment.

Perhaps this would not be an issue if the dota genre used strong narrative, visual, and mechanical backing for the decision. The goal is that you must explain "Why?" Why do you see the world from the perspective that you do? Many aspects of the dota camera—the degree of omnipotence available to the player, the top-down perspective—could be validated with the proper design choices.[^8] After all, recent games like The Last of Us, Dishonored, 2012's Syndicate, and Deus Ex: Human Revolution feature skills and tools for seeing through walls and the environment, and provide good reasons for why you can.

But proper craft requires proper execution, and the creators of dota games have half-assed the process. League of Legends asserts that you are a summoner who is in-fact controlling the action from a distance. The summoner role is the means by which you can view other parts of the battlefield and the means by which you control characters beyond the one you have chosen to play as. These games are simply borrowing the existing feedback mechanisms found in the RTS genre, where the characters you are bossing around acknowledge your existence and comment on your decisions. In other words, you're still playing the role of the commander, but with possession and control of an individual.

But if you are familiar with games such as Lifeline, Pac-Man 2: The New Adventures, Critical Path, Wirehead, Recettear: An Item Shop's Tale, a maligned game like Night Trap, or even the voice in the head of the main character in Deadly Premonition, then you know that you must take significant strides to convince players that it is worth playing a supporting role at the expense of the leading role. In order to do this, the supporting role must come to entirely dominate the mechanical and aesthetic conventions of your game. And very often, it must provide a distinctly different experience. Instead, the retroactive justification of the player's role in the dota games which use the free camera was simply to make the most of a bad situation, and it is disinteresting and nonsensical when compared to the strides taken by developers in other games and genres.

If you know your videogame history, you will know that it is only the dota genre which has struggled with the camera. The other half of the Warcraft III custom game scene that received the commercial treatment—the tower defense genre—has not. Many TD games maintain the same top-down perspective found in the maps built for Warcraft III and StarCraft. And that is perfectly fine, because traditional TD games are little more than simplified RTS games to begin with. But many developers correctly understood that TD games were simplified RTS games, and found that if they wanted to make their TD game anything less than a waste of time, then they had to attach the concept to another genre. In adopting the first-person shooter model, the Sanctum series plays from the first-person perspective. The Orcs Must Die! series has adopted the camera, interface, and control scheme more commonly found in MMORPGs. Those games used strong mechanical, visual, and narrative backing in order to explain why the game is being played from their new perspective, and since they did it well enough, nobody gave it a second thought.

Well beyond the walls of the dota genre, there have been countless videogames for both computers and consoles where the player manages elements typical to RTS and does it with a fixed camera. Games such as Herzog Zwei, Overlord, Giants: Citizen Kabuto, the Kingdom Under Fire series, AirMech, Brutal Legend, Guilty Gear 2: Overture, Ninety-Nine Nights, Mount and Blade, Battlezone, and even the Call of Duty series[^9] have demonstrated that it is possible to use a fixed camera to manage RTS elements. All of these games came from countless separate developers who were pursuing different styles of play, but all came to the same conclusion: RTS elements can be played from the ground level and they can be done very well.

"But Dota 2 and League of Legends require the precision of a point-and-click RTS game. How am I supposed to do this with a fixed camera?" Then I implore that you play Shiny Entertainment's Sacrifice, an action-strategy hybrid which has demonstrated with almost flawless fidelity that it is possible to manage RTS elements with a fixed camera. You can zoom and rotate the camera, but it is always locked to your summoner. The interface allows the player to control dozens of units at any time, and to control those units with the same flexibility found in other RTS games. Want to create formations? Want to send a unit halfway across the battlefield to defend a structure? Go for it. And yes, these concepts have been held to a high standard through the game's multiplayer modes, and are not just a cheap gimmick for use in a singleplayer setting. It's a third-person action game featuring all of the elements which are otherwise familiar to the Blizzard RTS games that birthed the dota genre. So before you say the concept can't work, go play Sacrifice and get back to me.[^10]

What this should demonstrate is that the removal of a free camera is not about "dumbing down" the genre. The goal in game design is to make sure your best moments and your most interesting ideas are better than the ones in competing games.[^11] To argue that the dota genre needs a free camera is to argue that the genre is doing things which are fundamentally more interesting with the free camera. But games like Sacrifice allow you to comfortably manage and control your troops from the third-person. Call of Duty: Black Ops II and Brutal Legend provide interesting narrative context for their RTS elements. And in the pursuit of this camera, the dota genre is losing support for the great ideas that would be more effective with a fixed camera, particularly the control schemes used by the classic action games for console and arcade hardware. To argue that the free camera is absolutely essential to the character of the genre—when there is no one thing that dota can do better with it—is to argue the genre isn't that interesting to begin with.

Then again, an "argument of merit" is secondary to the reason that a fixed camera meets incredible resistance. Does anyone believe that if the dota genre had been built for a fixed camera, players would be screaming that it is holding the genre back, and that developers should let everyone play dota like an RTS? Of course not. And if fans of dota are completely unconcerned with "immersion", and it is control of the battlefield that they desire, then how come they have not asked more powerful and more flexible cameras? Why haven't they demanded that the camera in 2009's Demigod become a universal standard for the genre, when Gas Powered Games adopted their Supreme Commander "strategic zoom" feature for use in a dota game?[^12] If we are to accept dota's narrative device at face value, and you are playing the role of an omnipotent wizard, it only makes sense that the user interface streamlines that omnipotence.

The simple answer is that dota players don't want any of these things, and the resistance to change is a common part of the hardcore videogame experience. To use a relevant example, take a look at when StarCraft II: Wings of Liberty was announced and revealed back in 2007. There was significant concern over the game's upgraded user interface, because it would allow players to select more than twelve units and select more than one building at any time. Much of the raw input required to play and master StarCraft is derived from the demands of its interface, and long-time fans argued the new interface would lead to reduced depth and a less enjoyable game.[^13] The choice to pursue the interface upgrades commonplace in RTS games made after 1998—most already present in 1997's Total Annihilation, 1997's Dark Reign, and the early Command and Conquer games—had become a heated point of contention across the StarCraft community.[^14] This is because the change was only being considered in relation to the original StarCraft. These players were willing to settle for an inferior, more restrictive interface because they were not familiar with the RTS games that had demonstrated superior concepts using their superior interfaces.

Much the same applies here. The insistence on the dota genre's current camera is about protecting a very specific game model that relies on the free camera as a means to skillful player input. If you allow players to manage the strategic picture from a bird's eye perspective, it will reduce the importance of player input and spatial awareness in the course of skilled play. In the face of top-down point-and-click action games which demand a much higher "Actions Per Minute"[^15], and in the face of games with far more moving parts, the genre desperately needs this mechanical interaction in order to remain interesting. The removal of the free camera and its limited field of view would lower the barrier even further. And instead of embracing the superior concepts that could be implemented with a superior camera, those players will reject it, for the fear and risk that comes with an "unknown quantity".

In the end, the defense of the camera amounts to "Don't change it, because you may break something."[^16] And in a medium which has been defined by a terrifyingly rapid evolution, that is never ever an excuse. Warcraft III map designers only pursued the free camera because the Warcraft III game engine made it the comfortable, easy choice. And today, players only accept the free camera because it is the comfortable, known commodity which the genre was built on.

So what I will tell you is this: If you think the free camera is the correct design choice, you are arguing that a series of map creators who lacked the creative resources and talent got it right. You are arguing that an amateur mapmaking community all made the same, "correct" decision in the pursuit of fundamentally different projects—dota games, tower defense, dungeon crawlers, or elsewise—which have traditionally demanded different interfaces and cameras. And you are arguing that the commercial game designers who had the creative and financial freedom to design their illusions from scratch got it wrong. Quite simply, the free-roaming camera was an overreach that was chosen because it had to be chosen, and was never complemented with the proper visual, narrative, and mechanical design decisions. The free camera is not essential to the experience, and countless excellent games have shown that in the context of a character-action game, it is the inferior option.

[^1]: It's a practice best exemplified by Nintendo, where it very often seems like the hardware is built for the _Mario_ game that will figurehead the platform.

[^2]: Lo and behold, it is commonly argued that in using _League of Legends_ as the blueprint, _Smite_ is using its fixed third-person perspective as a gimmick.

[^3]: Occasionally, you are inserting yourself in a role which exists outside of the game, whether match clear puzzle games like _Tetris_ or rhythm games like _Dance Dance Revolution_. You are a strongly-defined participant nonetheless.

[^4]: This is not to argue that these games have not attempted to subvert the established order from time to time. But if any of these games handle their camera poorly, it would not invalidate a line of theory which has been confirmed by the master craftsmen of the medium.

[^5]: It is a precedent which has already been confirmed and established through roughly two-plus centuries of tabletop wargaming.

[^6]: And eventually, the ideal for these games is that you will play the commander role from the first-person perspective, where you are sitting inside of the ship or vehicle and viewing the battlefield through the onboard technology. The simple fact is that it will be a hell of a lot cooler to look across from your monitor—which will be inside of the game world—and see a wall of tanks coming directly at you.

[^7]: This is the reason that the first-person camera will eventually become the ideal for all character-action games. It has not become today's standard because we do not have the technology to achieve those ends, and the third-person camera can provide the spatial awareness that is often limited in today's first-person action games. In spite of this, games such as _Mirror's Edge_, _Breakdown_, and _Maken X_ have shown that the concepts common to third-person action games are very possible in the first-person.

[^8]: Perhaps the best precedent would come from _Kingdom Under Fire II_, in which the player can switch between the ground-level view of their character and the top-down commander role common to RTS. The difference is that this game uses strong, defined design to make it happen, while dota feels sloppy and loose because the games are co-opting an existing body of theory (commander role) for a different purpose (character-action game).

[^9]: The Strike Force mode in _Call of Duty: Black Ops II_ is a strategy game mode where players control the strategic picture from a satellite view and take control of soldiers and drones in order to achieve tactical goals. In the world of _Black Ops II_, a world where computer technology is ubiquitous, a world where computer technology allows us to network with just about anything, it makes sense and feels completely natural. Even a game series considered the bottom of the barrel by many videogame players understood these lessons.

[^10]: Hell, I would recommend that you play _Sacrifice_ anyway, because it's fucking awesome. ([source](http://store.steampowered.com/app/38440/)) ([source](http://www.gog.com/game/sacrifice))

[^11]: This is the reason, for instance, that classic 2D side-scrolling games can maintain their appeal even as the industry pours billions of dollars into massive, open 3D worlds. Even if the new games have greater potential for interesting concepts and ideas, the 2D games are often presenting ideas and challenges that those 3D games are not.

[^12]: Well, other than the fact that the dota genre is very popular in developing nations, and that a "strategic zoom" feature would push consumer technology in places like Vietnam and Malaysia. But that's a topic we'll give more attention to later on.

[^13]: And yes, _StarCraft II_ may be a less enjoyable game, but it has nothing to do with the upgraded interface. The interface was the correct design choice and an obvious improvement. It was the failure of Blizzard Entertainment to adjust and redesign their game in order to account for that improvement, in-part because those changes would have also been rejected by the die-hards.

[^14]: In a 2007 TeamLiquid.net user-created poll asking how _StarCraft II_ should handle unit production, 42 percent of the 1100 respondents were in opposition of "Multiple Building Selection", the given term for the mechanic that would allow players to select multiple buildings and more efficiently produce their troops. Those opposed to the interface changes included top Western players such as—but most certainly not limited to—Dan "Artosis" Stemkowski and Greg "IdrA" Fields. ([source](http://www.teamliquid.net/forum/closed-threads/60555-poll-mbs-implementation-or-not)) ([source](http://www.teamliquid.net/forum/closed-threads/60202-petition-for-no-mbs))

[^15]: Actions Per Minute is the rate at which players can issue commands. Whether dota or RTS, beginners are usually in good shape if their APM is anywhere from 30 to 60\. Professional players typically end up somewhere in the range beyond 200\. While APM is commonly held as a broad measurement of skill in RTS games, veteran players understand that the skill is in making sure your actions are more efficient and impactful than those of your opponents.

[^16]: And no, you idiots, I am not proposing that you inject the fixed camera directly into _Defense of the Ancients_, _Dota 2_, _League of Legends_, or _Heroes of Newerth_. Remember: This book is intended to discuss broad concepts, and this is one of the broad concepts that has met incredible resistance, regardless of whether the change is proposed for a new game or an old game.