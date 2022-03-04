---
title: "January 19th, 2021 Livestream Q&A: While Unreal Engine 4 gets upgraded, will the Object Limit get changed?"
date: "2021-01-19"
layout: transcript
topics:
    - "satisfactory-updates/released/satisfactory-update-4"
    - "technology/unreal-engine/object-limit"
---
# [January 19th, 2021 Livestream](../2021-01-19.md)
## Q&A: While Unreal Engine 4 gets upgraded, will the Object Limit get changed?
https://www.youtube.com/watch?v=BE6kB3nmSdM
This question was possibly duplicated with a more recent answer: January 26th, 2021 Livestream Q&A: Will you tell here the current build limit number considering the Engine Upgrade? [https://www.youtube.com/watch?v=WfU45N1EvQ0](https://www.youtube.com/watch?v=WfU45N1EvQ0)


### Topics
* [Satisfactory Updates > Released > Satisfactory Update 4](../topics/satisfactory-updates/released/satisfactory-update-4.md)
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> while unreal engine 4 gets upgraded with the block limit change as well so the the block limit i think i assume you're referring to the memory limit that's exists for the garbage collector in unreal engine, it depends if they've updated it if they haven't updated that then no, it's it's, it's a limitation the the whole like build limit thing that's not something that we've set that's something that exists in a real engine it's a limitation to their implementation of the garbage collector and that limitation is there to protect memory with the game, so i see a lot of threads where people like are upping that build limit and you can do that but that makes the game potentially very unstable, it's it's not a matter of like you know if i have enough ram i can i can totally do it like that's not how that works at all, it has to do with like how the sizes of data allocation and stuff like that and that's not affected by ram whatsoever, and you can do that but you can you can run into very severe issues if you do do that which i mean you can do that if you want but if you do increase the the object limit which is the you object limit not the build object limit then be aware that your save file make it corrupt it strange glitches can appear and the game can like randomly crash or stuff like that and i've talked to people that had corrupted saves after doing this so i know it happens so make sure to backup your saves if you do, just so you know but, we are working on optimizing the the amount of object data objects are that are in the game itself, and that will decrease like how much we're actually using out of that limit so it's not like we can never improve on that there's always improvement we can't actually up the limit we have to optimize the game for it rather than, so that's the long answer to that question
