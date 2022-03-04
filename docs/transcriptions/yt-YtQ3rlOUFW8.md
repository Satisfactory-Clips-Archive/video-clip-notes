---
title: "February 22nd, 2022 Livestream Q&A: Increase Object Limit, when?"
date: "2022-02-22"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [February 22nd, 2022 Livestream](../2022-02-22.md)
## Q&A: Increase Object Limit, when?
https://www.youtube.com/watch?v=YtQ3rlOUFW8
<details>
<summary>This question may have been asked previously at least 2 other times, as recently as November 2021 and as early as August 2021.</summary>

* [November 16th, 2021 Livestream Q&A: Are you guys going to increase the build limit now that we can place more items?](./yt-TGuLDBd8Wao.md) [https://www.youtube.com/watch?v=TGuLDBd8Wao](https://www.youtube.com/watch?v=TGuLDBd8Wao)
* [August 31st, 2021 Livestream Q&A: Build limit in Update 5?](./yt-JuzKAS5cvOQ.md) [https://www.youtube.com/watch?v=JuzKAS5cvOQ](https://www.youtube.com/watch?v=JuzKAS5cvOQ)
</details>


### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> increase object limit when so, never we can actually say that for sure because the object limit isn't something that we've set this is not something that we can control either because it's something that is part of the engine, and you know the engine isn't really intended to be used the way we use it, it's it has to do with how the memory is managed, in the engine and like you can sort of up that limit using config files and that's been possible ever since day one but, the problem is that like there's no there's like you're kind of like losing out on safeguards when you do that so like a lot of weird things can happen memory wise if you start you know changing that number, because that is a theoretical limit, so like there's been people reporting that like they've had their save files corrupted or you know like weird stuff happening factory logic not working the way they should, so it is always recommended that we don't change that we are however working on improving the game so we don't have to use as many game objects now a game object isn't the same as like an object that you place in the world it has a memory object specifically so like if you place a constructor for instance it used to be that a constructor was like maybe 16 different game objects and now it's like down to eight and i think there's plans to improve that as well and like maybe not specific for the constructor but like for a lot of different things we are constantly working on improving the memory footprint of the game and, i believe recently we've been working a lot on like the environment to like kind of get down the memory footprint on that and like how we manage loading the environment and stuff like that, so, but we can't really change the the like the u object limit the unreal object limit, that's set by the engine
