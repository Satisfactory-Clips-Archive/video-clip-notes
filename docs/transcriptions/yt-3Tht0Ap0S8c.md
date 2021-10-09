---
title: "November 10th, 2020 Livestream Q&A: Is there a debug command to see how many Objects you are using?"
date: "2020-11-10"
layout: transcript
topics:
    - "features/unplanned-features/mass-building"
    - "technology/unreal-engine"
---
# [November 10th, 2020 Livestream](../2020-11-10.md)
## Q&A: Is there a debug command to see how many Objects you are using?
https://www.youtube.com/watch?v=3Tht0Ap0S8c
This question was possibly duplicated with a more recent answer: [March 23rd, 2021 Livestream Q&A: Object Limit, any chance to display how much is left somehow?](./yt-SNPdVSInCCQ.md) [https://www.youtube.com/watch?v=SNPdVSInCCQ](https://www.youtube.com/watch?v=SNPdVSInCCQ)


### Topics
* [Features > Unplanned Features > Mass Building](../topics/features/unplanned-features/mass-building.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> sir uh is there a debug command to see how many objects you're in uh the game is using that's interesting i wonder if there's a way we could like give them that information so they have some idea i don't know if there's even a way for us to do that yeah well possibly but i don't know yeah i don't think so because a lot of like debug stuff is baked out of the build because it takes up a lot of uh space in the building um so a lot of tools we use to track that stuff isn't really do like it's not good to bake it into the game because it leaves a big footprint for you guys uh even the fact that we use uh because right now we're baking in the uh symbols also for our error tracking so whenever the game crashes for you you'll get like the call stack and stuff that's like four gigs of the game or something that's just used for that for just helping us debug it like the game would be significantly smaller if we just remove that but
