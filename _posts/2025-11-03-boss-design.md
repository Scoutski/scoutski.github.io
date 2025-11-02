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

I love boss fights - some of my favourite games of all time are defined by their boss fights. I would include things like the God of War series (controversially, I didn't enjoy Ragnarok very much because I didn't like the boss fights...), Souls games and Hollow Knight/Silksong. There's something so satisfying about mastering a series of patterns and identifying safe windows and executing efficiently. I kind of feel like boss fights are mini-rhythm games, your goal is to get in time with the notes the boss is playing and react accordingly. I have not applied a game designers hat to boss fights as much as I could at this point but today I'm going to break down some of the things I love in different boss fights and then work out what I can apply to my game.

## Boss mechanics

### Teaching the player about a newly acquired mechanic

![Desktop View](/assets/img/week-1/dodongo.jpg){: width="445" height="250" }

A common tactic with bosses is to use them as a skill check for the player. Take for instance the game "The legend of Zelda: Ocarina of time", many of the dungeon bosses will take whatever new mechanic the player is given in that dungeon and will be pivotal to actually defeating that boss. In this case, let's look quickly at King Dodongo in the Dodongo's Cavern dungeon.

This is the second dungeon in the game and at this point the player has very few tools in which they can use to fight back. The tool that the player is given in this dungeon is bombs which the player can place on the ground, after a short delay highlighted by an increasing flashing red telegraph will explode, allowing the player some skill expression through correct timing.

Dodongo in question will curl up in to a ball and roll around the arena, the goal for the player is to then time placing their bombs down correctly so that they explode while he rolls by, rewarding the player with a "stunned" phase and they can get some free hits with their sword.

The entire fight is just repeating this process and letting them master their timing and use of the bombs. Other bosses in the game continue to follow this pattern of teaching the player and rewarding them for their mastery. The best execution of this pattern is when larger scale bosses (sometimes just the final boss), require the player to reuse all the skills they've learned through different bosses together in a single fight. In a way it's kind of like a final exam that allows the player to prove their mastery across all the skills they've learned throughout the game.

One other addendum is that often the mechanic will first be taught more safely against individual enemies before a larger challenge is presented with the next boss.

100% focus for individual enemy -> 100% focus for Boss -> 10% focus on Final Boss

As far as my game is concerned, I think multiple skills are not really in scope for what I'm trying to achieve but I love this pattern and if I were to make a bigger game I would absolute use this approach.

### Cycling between different moves

![Desktop View](/assets/img/week-1/last-judge.avif){: width="800" height="450" }

Often a boss will simply cycle between a predetermined list of "available moves", depending on the complexity of the game, this is sometimes true of individual enemies. On the player's side of thing, the plan is that they are given a manageable set of moves to learn (again thinking of a dance/rhythm game here) which will be cycled consistently until the boss is either defeated, or a new phase (next section) is reached.

This part of the design seems to be integral to managing an appropriate level of difficulty. Earlier in a game, a boss is likely to only have around 2 moves per phase as the player is still likely mastering the controls of the game while also allowing them to feel capable and strong so they can lean on their early successes when they reach the more challenging bosses later in the game.

I do think this is kind of a standard approach that would exist for almost every boss in every game. I definitely want to apply a cyclable move set to a boss/bosses in my game, in some cases bosses are allowed to repeat the same move from a random set, but I find it more enjoyable if the same move is never repeated, so my approach will be:

- Create 3 different moves
- After one has completed, choose randomly from the other 2 moves and complete that move
- Repeat.

Ideally each move would test a different player ability (dodging/reacting/shooting a weak spot). In the case of my game, there aren't that many player abilities to take advantage of but the moves I have in mind are:

- Boss moves left and right on the top of the screen and shoots bullets in a zig zag pattern for the player to dodge between.
- Boss moves to the center of the screen and shoots out two streams which wipe back and forth across the screen.
- Boss indicates with a path a charge and then with appropriate delays charges at the player 3 times before returning to the top of the screen.

### Multiple phases

![Desktop View](/assets/img/week-1/malenia.webp){: width="690" height="388" }

Phases are an extension of different moves and just make a boss fight feel bigger and more epic for the players. A lot of the time, early game bosses won't have vastly different phases, a pattern sometimes used is at a specific health breakpoint, they will complete the same moves as the first phases but at an increased speed, allowing the player to continue to show mastery at an increased speed.

I used the Mantis lords from Hollow Knight as the header image for this post which are a great example of this, after completing the first phase of the fight against a single one of the lords, they return to their throne and the player is challenged by the other two lords at the same time while using the exact same move set. Many players consider this fight one of the most enjoyable fights from the game due to the feeling of mastery over the course of the fight. In fact, players were gifted in the Godhome DLC (boss rush mode) with a version of the fight called "Sisters of battle" which was the same again but had the player tackle all 3 of the characters at once.

Later in games, phases are defined by a completely different moveset to the first phase, sometimes with an entirely new health bar (very common in souls games). Take for instance the image for this section, Malenia from Elden Ring. This fight is well-known for it's difficulty and for many players who struggled to get over the difficulty of the first phase of the fight, were presented with an entirely new phase where she had increased mobility and additional moves. At first this phase shift can be very overwhelming but in this case (and many of the ones I love), the moveset is an extension of the moves used in the first half that present slightly differently, with a slightly added attack or are almost completely the same.

![Desktop View](/assets/img/week-1/waterfowl.gif){: width="360" height="180" }

That said, this process of extending the first phase and building on that moveset is not always used, take the King of Puppets fight from Lies of P which does away with this completely. The first phase of the fight is a giant enemy with impactful, heavy, slow moves before transitioning in to a fight against a human sized opponents with nimble, quick, multi-hit moves. My personal preference leans against this kind of boss fight as I believe it punishes a player in the second phase by switching up the fight rather than building on the confidence they built in the first half. That's purely an opinion though and there are no hard rules about how phases should be handled.

In the case of my game, I am currently planning on creating 3 different levels, each with a different boss at the end. Multiple phases may be a bit hard to implement for all of them, especially as that would be more punishing for a player at the end of each level. I think I love this aspect of boss design though and for the 3rd boss I'd like to include at least a second phase for that one with the goals being:

- More memorable final fight with properties that separate it from the previous two bosses.
- A chance to extend a moveset between phases.

### Spawning additional enemies

![Desktop View](/assets/img/week-1/coneflies.png){: width="500" }
<!-- ![Desktop View](/assets/img/week-1/coneflies.png){: width="1233" height="694" } -->

There's a lot of value in creating additional challenges to cause the player to split their focus where they have to rely on multitasking between watching the boss, reacting to it's moves while also completing a secondary objective. This was a pattern applied consistently across Hollow Knight: Silksong. There are a few things that can make a big difference between a good challenge and frustration.

The first kind is the way the Raging Conchflies boss is executed. During the fight, the boss spawns small coneflies that essentially perform the same attack as the bosses, they find a fixed position on one side of the screen and then one after each other, will fly towards the player in a predictable manner, followed immediately by the bosses themselves.

![Desktop View](/assets/img/week-1/beastfly.png){: width="400" }

The other kind can be seen with the Savage Beastfly fight. This fight is viewed incredibly differently from the playerbase (There is literally a [subreddit dedicated to hating this bossfight](https://www.reddit.com/r/fucksavagebeastfly/) which as of writing has 42000 weekly visitors). Rather than predictable enemies, the additional enemies spawn as part of the bosses move rotation and then act independently of the boss. This approach leads to frustration and taking away agency from the player who can't accurately predict and prepare what's ahead of them as the unpredictability of different enemies performing moves regardless of each other can lead to many unwinnable/undodgeable situations. Although this fight in particular wasn't popular,

### Environmental hazards

Depending on the type of game, the boss arena is a hazard in itself which the player must manage just as much as the boss

### Telegraphs

### Hit registration

