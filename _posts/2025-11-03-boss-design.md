---
title: "Week 1 - Boss design!"
date: 2025-11-03 07:25:00 +1100
image: /assets/img/week-1/mantis-lords.webp
published: true
categories: [design, ideation]
tags: [design, ideation]
---

Hello there!

It was a bit of a busy week for me last week and I needed a little break after rushing through the Laser Defender tutorial. I really wanted to get this week started on the right foot and so have decided to do so by tackling probably the thing I find the most fun.

I love boss fights - some of my favourite games of all time are defined by their boss fights. I would include things like the God of War series (controversially, I didn't enjoy Ragnarok very much because I didn't like the boss fights...), Souls games and Hollow Knight/Silksong. There's something so satisfying about mastering a series of patterns and identifying safe windows and executing efficiently. Boss fights are mini-rhythm games, your goal is to get in time with the notes the boss is playing and react accordingly.

In the past, I have not applied a game designers hat to boss fights but today I'm going to break down some of the things that I notice (and love) and then work out what I can try to apply in future.

## Boss mechanics

### Teaching the player about a newly acquired mechanic

![Desktop View](/assets/img/week-1/dodongo.jpg){: width="445" height="250" }
_King Dodongo from The Legend of Zelda: Ocarina of Time._

Bosses often act as a skill check for a new ability acquired by the player. Take for instance the game The legend of Zelda: Ocarina of time, many of the dungeon bosses will take whatever new mechanic the player is given and make it the key to defeating that boss. In this case, let's look quickly at King Dodongo from Dodongo's Cavern.

This is the second dungeon in the game and at this point the player has very few tools in which they can use to fight back. The tool given in this dungeon are bombs, which the player can place on the ground and after a short delay highlighted by an increasing flashing red telegraph, will explode. This allows the player some skill expression through timing their placement correctly.

During the fight, King Dodongo will curl up in to a ball and roll around the arena. The goal for the player is to place their bombs down so that they explode while he rolls by, rewarding the player with a "stunned" phase where they can get some free hits in.

The entire fight repeats this process and lets them master the timing and use of the bombs. Other bosses in the game follow this pattern of teaching the player and rewarding them for their mastery. The best execution of this pattern is when larger scale bosses (sometimes just the final boss), require the player to reuse all the skills they've learned through different bosses together in a single fight. In a way, it's kind of like a final exam that allows the player to prove their mastery across all the skills they've obtained throughout the game.

Oftentimes, the mechanic will first be taught more safely against individual enemies before a larger challenge is presented with the next boss.

100% focus for individual enemy -> 100% focus for Boss -> 10% focus on Final Boss

As far as my game is concerned, I think multiple skills are not really in scope for what I'm trying to achieve but I love this pattern and if I were to make a bigger game I would absolute use this approach.

### Cycling between different moves

![Desktop View](/assets/img/week-1/last-judge.avif){: width="800" height="450" }
_The Last Judge from Hollow Knight: Silksong._

Bosses typically will cycle between a list of available moves, depending on the complexity of the game, this can be true of individual enemies as well. On the player's side of things, they are given a manageable set of moves (I can't stop thinking of a dance/rhythm game here) which will be cycled consistently until the boss is either defeated, or a new phase (next section) is reached.

This part of the design seems to be integral to cultivating an appropriate level of difficulty. Earlier in a game, a boss will often have around 2 moves per phase as the player is still likely mastering the controls of the game, while also allowing them to feel capable so they can lean on their early successes when they reach the more challenging bosses later in the game.

I do think this is kind of a standard approach that would exist for almost every boss in every game. I definitely want to apply a cyclable move set to a boss/bosses in my game, in some cases bosses are allowed to repeat the same move from a random set, but I find it more enjoyable if the same move is never repeated, so my approach will be:

- Create 3 different moves
- After one has completed, choose randomly from the other 2 moves and complete that move.
- Repeat.

Ideally each move would test a different player ability (dodging/reacting/shooting a weak spot). In the case of my game, there aren't that many player abilities to take advantage of but the moves I have in mind are:

- Boss moves left and right on the top of the screen and shoots bullets in a zig zag pattern for the player to dodge between.
- Boss moves to the center of the screen and shoots out two streams which wipe back and forth across the screen.
- Boss indicates with a path a charge and then with appropriate delays charges at the player 3 times before returning to the top of the screen.

### Multiple phases

![Desktop View](/assets/img/week-1/malenia.webp){: width="790" }
_Malenia, Blade of Miquella from Elden Ring._

Phases are an extension of different moves and just make a boss fight feel bigger and more epic for the player. Early game bosses won't typically have vastly different phases. Often, at a specific health breakpoint, a boss will complete the same moves as the first phases but at an increased speed, allowing the player to continue to show mastery with less margin for error.

The Mantis lords from Hollow Knight are a great example of this, after completing the first phase of the fight against a single one of the lords, they return to their throne and the player is challenged by the other two lords at the same time while using the exact same move set. Many players consider this fight one of the most enjoyable fights in the game due to the feeling of mastery over the course of the fight. In fact, players were gifted in the Godhome DLC (boss rush mode) with a version of the fight called "Sisters of battle" which was the same again but had the player tackle all three of the Mantis' at once.

In the later parts of some games, phases are defined by a completely different moveset to the first phase, sometimes with an entirely new health bar (very common in souls games). Malenia from Elden Ring is well-known for her difficulty and for many players who struggled to get over the difficulty of the first phase of the fight, were presented with an entirely new phase where she had increased mobility and additional moves. At first this phase shift can be overwhelming but in this case (and many of the ones I love), the moveset is an extension of the moves used in the first half that present slightly differently, with an added attack, or are almost completely the same.

![Desktop View](/assets/img/week-1/waterfowl.gif){: width="360" height="180" }
_Malenia's most famous move: The waterfowl dance._

That said, this process of extending the first phase and building on that moveset is not always used. The King of Puppets fight from Lies of P does away with this completely. The first phase of the fight is a giant enemy with impactful, heavy, slow moves before transitioning in to a fight against a human sized opponents with nimble, quick, multi-hit moves. My personal preference leans against this kind of boss fight as I believe it punishes a player in the second phase by switching up the fight rather than building on the confidence from mastering the first half. That said  there are no hard rules about how phases should be handled.

In the case of my game, I am currently planning on creating 3 different levels, each with a different boss at the end. Multiple phases may be a bit hard to implement for all of them, especially as that would be more punishing for a player at the end of each level. I think I love this aspect of boss design though and for the 3rd boss I'd like to include at least a second phase for that one with the goals being:

- More memorable final fight with properties that separate it from the previous two bosses.
- A chance to extend a moveset between phases.

### Spawning additional enemies

![Desktop View](/assets/img/week-1/coneflies.png){: width="790" }
_The Raging Conchflies from Hollow Knight: Silksong._

There's a lot of value in creating additional challenges to cause the player to split their focus where they have to rely on multitasking between watching the boss, reacting to it's moves while also completing a secondary objective. This was a pattern applied consistently across Hollow Knight: Silksong. However, there are a few things that can make a big difference between a good challenge and frustration.

The first kind van be seen with the Raging Conchflies boss. During the fight, the boss spawns small coneflies that essentially perform the same attack as the bosses, they find a fixed position on one side of the screen and then one after each other, will fly towards the player in a predictable manner, followed immediately by the bosses themselves. This results in a pattern where the player can recognise and consistently react to what is coming at them, rather than having to deal with the chaos of individual entities acting independently.

![Desktop View](/assets/img/week-1/beastfly.png){: width="400" }
_Savage Beastfly from Hollow Knight: Silksong._

The other kind can be seen with the Savage Beastfly fight. This fight is viewed incredibly harshly from the playerbase (There is literally a [subreddit dedicated to hating this bossfight](https://www.reddit.com/r/fucksavagebeastfly/) which as of writing has 42000 weekly visitors). Rather than predictable enemies, the additional enemies spawn as part of the bosses move rotation and then act independently of the boss. This approach leads to frustration and taking away agency from the player who can't accurately predict and prepare for what's ahead of them. The unpredictability of different enemies performing moves independent of each other can lead to many unwinnable/undodgeable situations. Although, this example wasn't a popular fight, I do think there is room for this kind of design, as long as the player can feel agency during the fight and that their own skill expression is responsible for their victory as opposed to luck and timing.

I do think this is a great boss pattern and would love to include additional enemies spawning as part of the final boss in my game. I'd love to do something that suggests they are either coming to the defence of the boss OR the boss is the supreme commander and they are acting in service of them.

### Environmental hazards

![Desktop View](/assets/img/week-1/lady-butterfly.webp){: width="790" }
_Lady Butterfly from Sekiro: Shadows die twice._

Although very similar to adds, environmental hazards present an additional challenge for the player and in many cases can be used to help build the emotion of a fight. Some simple examples of this kind of thing are including spikes, lava or moving platforms.

The Lady Butterfly fight from Sekiro: Shadows die twice is an example that has simple hazards, fire all over the ground that spawns based on falling beams from above. The cool part about the hazards here is that it builds a different kind of tension and storytelling in the fight. It takes place in a burning building and as the fight goes on, more fire/wood spawns on the ground, giving the player a sense that they are fighting against the clock as well as the boss (as far as I recall there isn't an actual timer on the boss fight though).

In my case, I would consider using some kind of flying space debris as obstacles for the player. These would be immune to damage (or take a significant and inneficient amount of fire) that creates a dodging challenge for the player while also managing the moveset of the boss.

### Arena design

![Desktop View](/assets/img/week-1/saintsword.webp){: width="790" }
_The Isshin: Sword saint arena from Sekiro: Shadows die twice._

Similar to environmental hazards, the actual arena of a boss fight can add a huge amount of flavour to a boss fight and make it memorable. There's a lot of bosses that came to mind for this one, but the one that really sticks in my mind is Isshin, the sword saint from Sekiro: Shadows die twice.

This fight uses a classic kind of Japanese imagery of a fight between Samurai in a field of long grass under a full moon. As this is a multi-phase fight, the intensity of the environment builds with the intensity of the fight. By the end, there are huge lightning streaks across the sky. Strong winds blow the long flowers/grass in all directions and as a player you feel that the arena is reacting to the intense clash taking place.

Another type of arena design that can be seen sometimes (for example: The stranger at the start of God of War (new series), or Lady Butterfly again) is a deteriorating area over the course of the fight. When the world seems to be reacting to the player's actions, it leads to a sense of power on the part of the player and tells an epic story for the course of the fight.

Unfortunately as much as I'd love to do something like this, it may be outside the scope of a small game 1, but I want to recognise the importance of good arena design and how it can make a fight more memorable for the player.

### Telegraphs

![Desktop View](/assets/img/week-1/ffxiv-boss.jpg){: width="790" }
_A FFXIV raid showing arena warnings on the floor (I don't know which boss this is)._

In order for a boss fight to feel fair, a player must feel like they have the opportunity to react in a reasonable amount of time and have some sense of what's coming. The two main ways that telegraphs are presented are with arena warnings and then wind up animations.

In Final Fantasy XIV, raid bosses often have the floor painted with safe or unsafe areas, showing the player where they have to move and then giving them a few seconds to get in to position. This allows players to feel that they had the opportunity and warning if they end up getting hit. If a boss has a sequence of attacks, it can also give them a series of actions in a row to prepare for.

Wind up animations are a staple of Fromsoft games, usually a boss will pull their weapon back slowly before slamming down in front of them. One very important aspect of these animations is that each wind up should look distinctly different from one another. The player can then with practice, understand exactly what attack is coming and react accordingly.

As a final note, I was trying a demo recently for a game in progress that featured metroidvania-style boss fights. Although most of the game felt fun and the controls felt good, there was a distinct lack of telegraphs during the boss fight which made me immediately feel a bit powerless and frustrated. The game didn't feel like it was giving me a chance to figure it out and that I'd be relying on luck or the timing window after an attack rather than being predictive and being rewarded accordingly.

Telegraphs are universally useful and I plan to make use of arena warning for attacks that warrant them.

### Hit responsiveness

![Desktop View](/assets/img/week-1/nergigante.png){: width="790" }
_An injured Nergigante flees from a player in Monster Hunter: World._

In most games, an enemy reacting to the actions of a player is important to show the player that what they are doing has impact and that the game is recognising their actions. The games that do this the best have to be the Monster Hunter series.

During a fight against a target monster, the monster slowly develops injuries, loses body parts and eventually begins limping. In the screenshot above you can see a Nergigante which has had the end of it's tail removed as a result of all the damage it's taken.

It's important for a player to feel like they're making progress with something other than watching a health bar go down. Sometimes this can be done with different phases that change the action, but building up injury/damage on the actual model is a great way to make the player feel strong and that they are making progress.

One other aspect of hit responsiveness are the on-hit effects. In games with bigger slower attacks, sometimes the boss will stagger or step back from a big hit. On the other hand, it can make the fight too easy if the boss is interrupted everytime they are hit, but things like splashes of blood, or in 2D games, flashing the enemy on hit just to show the player that what they are doing is working can be just as useful.

I plan to make use of the flashing enemy on hit and a deteriorating model (probably just a second one, halfway through the fight). I think hit responsiveness is super important and it makes fights feel so good when the player feels like their actions are being felt by the enemies.

### Scale

![Desktop View](/assets/img/week-1/titan-ffxvi.webp){: width="790" }
_Titan from Final Fantasy XVI._

Scale through the environment or the opponent is another element that builds a memorable fight. Titan in Final Fantasy XVI has a sequence of cutscenes that really show off the size difference as the player is forced to run at high speed towards the mountain of a boss.

Although scale isn't always applicable depending on the type of game, it's another tool in the toolbox to allow the player to feel powerful and that they can overcome any odds in a David vs Goliath style battle. However there's not too much to say about how to implement scale as long as the design of the boss itself emphasises the scale difference well. This can be achieved with big, slow, impactful moves that feel like they would destroy the player in a single hit (even if they don't). Some games that do this quite well are God of War, World of Warcraft and probably the best of them all, Shadow of the Colossus.

I do plan to make the final boss of the game feel extra big in an effort to build a sense of epicness to the final fight, but in a vertical shoot'em up, I think it will be difficult to focus on the scale difference of a large enemy.

### Story implications + Build up

![Desktop View](/assets/img/week-1/shodan.avif){: width="790" }
_SHODAN, the primary antagonist from System Shock II._

The last point I'll talk about is how the player feels about a fight in relation to the game as a whole. Many games will give the player a reason to buy in to the stakes of their game world and the build up to the final battle with a main antagonist. Some examples are the boss killing the protagonist's family and friends, constantly taunting the player or otherwise just making their presence felt throughout the game.

A classic example is SHODAN from System Shock II. In this game, the player is trying to defeat a rogue AI who has taken over a starship that has been infected. Throughout the entire game, SHODAN's face appears on screens all over the levels, while constantly taunting the player. Most importantly they are making their presence felt to the player so that when you finally reach the ultimate showdown, they've felt it building in a way that makes them feel ready to take her down.

This is a harder element to achieve in a shorter, more arcade style game but I'd like to try provide some kind of story reason for the player to want to take down the bosses at the end of each level.

## Conclusions

Rather than taking any of the individual elements to turn something in to nothing. It's the cohesion of all the above points that make for the most memorable and engaging boss fights. As games move forward as a medium, many of these elements become staples and have strong expectations and are requirements for boss fights to feel fun for the player.

With that in mind, bosses are the most exciting part of any video game to me and I want to work hard to incorporate all of the above into my boss designs.

Thanks for taking the time to read!