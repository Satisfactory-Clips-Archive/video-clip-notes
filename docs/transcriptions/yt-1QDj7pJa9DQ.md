---
title: "October 9th, 2020 Livestream Snutt & Dylan Talk: Crash reporting"
date: "2020-10-09"
layout: transcript
topics:
    - "coffee-stainers"
    - "features/multiplayer"
    - "technology/unreal-engine"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Snutt & Dylan Talk: Crash reporting
https://www.youtube.com/watch?v=1QDj7pJa9DQ

### Topics
* [Coffee Stainers](../topics/coffee-stainers.md)
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> suspicious yeah i know it's planned i'm getting a bunch of arrows over here i'm trying to in case you're wondering i'm just clicking through this thing freaking out at me holy have to fight this guy in a error it's going nuts is going nuts is that the editors no yeah that's the insurer let's see what kind of crash you get here if you get that crash thing oh wait no everybody i was like you can show the crash report thing but i just realized everybody gets that yeah like look at how cool this is but did they get the, , do you want to report this to a programmer oh crashed is that something custom we've done it's something you can enable in the engine i think okay i think steak did it yeah i i don't think anyone's ever used it no i i actually it's funny because it usually just annoys me when i'm programming i don't know what the process is to hook up to what we're talking about right now is we have a setting enabled for like if an artist is like working and they get a crash they get like a pop-up that asks like hey do you want a programmer to debug this because one big problem with, bugs is that they're really hard to reproduce, oh yeah sometimes unless you can reproduce a bug while you're debugging it you have no way of knowing what's wrong so one instance of this was for instance when i was working on replication and people would get like a weird thing where the game would crash, out of nowhere when they're playing multiplayer essentially and it has something to do with like when a level was streamed out on clients but the server thought that actor was still alive, that was that was impossible to reproduce, and i essentially needed the like the i needed to to be able to reproduce it so i could debug it to be able to find out what happened and i i managed to do it once ever i had to guess how to fix that issue do you want to know something funny no they fixed that they fixed that yeah i know the one of the things related to that was like yeah we have to wait until the next, replication graph update yeah so i just did a workaround, until that update was in so that was i was i knew about that okay i'm missing something or rather my fix was that we have to update engine but until then let me just add a bit of an extra thing here that make sure it doesn't crash it's all that was a that was, if you look up like, duct tape, fixes that's one of them
