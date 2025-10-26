---
title: "Week 0 - Digging in on game one"
date: 2025-10-26 15:12:00 +1100
image: /assets/img/week-0/brainstorm.png
published: true
categories: [gamedev, ideation]
tags: [ideation]
---

Hello again!

## Intro

So I've spent a bit more time thinking about it over the last 2 days and looking at the experience levels of others participating in the course and think I should land myself firmly in Game 1 territory. The main reasons are:

- Primarily, I want to aim towards giving myself the win of creating something. I want to build my own confidence in my ability to follow through on the processes involved with this course.
- On the flip side, there's a risk that if I overshoot on complexity and fail, I lower my own self-confidence in my ability to finish something.
- I will actually have a realistic chance of having a developed prototype by the end of 7 weeks that I'm likely able to get more meaningful feedback on.

So that brings me back to the raptor-clone type game, I'm not 100% sure but I believe the genre would be more aptly named as a vertical-scrolling shoot'em up. We've been told that for a game at this level, we shouldn't be trying to innovate too deeply and make sure we can progress through our unknown unknowns, that said, there's plenty of ideas I have that I will give myself as stretch goals, because putting my own spin on something is probably where the most fun is.

![Desktop View](/assets/img/week-0/weapons-doodle.jpg){: width="810" height="1080" }
_Spent last night doodling on the couch with some weapon ideas._

As a basic outline for the game and what I expect would make it feel "complete", here's what I'm going to initially put down as the must-haves.

## Scope

### Game feel

Overall with an action/shooter type game, the player should feel engaged and powerful, they are going to be controlling a single character against an army. They should feel tense but motivated to destroy enemies and reach the end of a stage. This should revolve between periods of more intense enemy pressure and short "give me" sections where the player is allowed to flex their power.

### Technical details

- Ability for player to control ship and move around the screen in 4 directions while facing forwards.
- Ability for player to shoot single bullet forward, either on click, or with autofire (I think autofire is what I'm leaning towards).
- Ability to upgrade existing weapon to shoot 2 bullets at once instead of 1.
- Ability for enemy prefabs (Will start with 2) to spawn in offscreen and head either south through the screen or directly at the player.
    - Enemy one will fly in a line across the screen, starting from anywhere around the player and initially aiming for them but keeping a line.
    - Enemy two will only spawn from the top of the screen and will try to head directly to the player location.
- Ability for player to take damage from enemy collision or enemy weapon collision.
- Transition between two levels upon reaching the end of a stage.
- A Boss character that stays with the player on screen until defeated.
    - Single phase moving left and right at the top of the screen and shooting multiple bullets across the screen (think baby's first bullet hell).
- All characters and background should have art (maybe pixel drawn by me, or from a pack).
- Game elements should play appropriate sounds (e.g. gun firing, enemy dying, level music, etc...).
- UI elements:
    - Screens:
        - Menu screen
        - Pause screen
        - Game over screen
        - Victory screen
    - Elements:
        - Remaining player lives
        - Current weapons/upgrades
        - Score (total kills?)
        - Boss HP

### Stretch goals

> I just want to strongly reiterate that these goals are based in desire and not reality, if I complete any of them I will be quite happy, but won't get fixated on including them.
{: .prompt-warning }

- Additional weapon types (such as the ones in the doodle I posted).
- Additional enemy types.
- Multiple bosses.
- A campaign map with level selection where a player can choose to go one of two ways and end up fighting optional bosses.
- Some kind of persistent data between runs, e.g. scores or super stretch goal, upgrades.
- The ability to save a run in progress and continue from where you left off.

## Closing

That feels like a solid starting point and I imagine I'll get the chance to get feedback on it before I begin in case I'm being either too bold or not bold enough. I'm excited at the potential and look forward to having friends play it for me, but realistically this is not a project I expect to be trying to sell to anyone. I want to reiterate for myself that the purpose of this project is to learn the process and complete something, after that point I hope to harness the knowledge on future projects where I aim for greater complexity.

The course starts tomorrow morning at 7 am and I can't wait to get started! Thanks for having a read!

Mike