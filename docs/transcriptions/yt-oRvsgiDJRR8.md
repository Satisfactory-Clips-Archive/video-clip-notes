---
title: "May 25th, 2021 Livestream Q&A: Can you talk about multi-threading?"
date: "2021-05-25"
layout: transcript
topics:
    - "coffee-stainers/ben"
    - "features/buildables/conveyor-belts"
    - "features/buildables/lights"
    - "features/buildings"
    - "features/fluids/pipes"
    - "technology"
---
# [May 25th, 2021 Livestream](../2021-05-25.md)
## Q&A: Can you talk about multi-threading?
https://www.youtube.com/watch?v=oRvsgiDJRR8

### Topics
* [Coffee Stainers > Ben](../topics/coffee-stainers/ben.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)
* [Features > Buildings](../topics/features/buildings.md)
* [Features > Fluids > Pipes](../topics/features/fluids/pipes.md)
* [Technology](../topics/technology.md)

### Transcript

> can you talk about multi-threading i can talk about multi-threading, that's that's sort of what the stream is for, so the game has multi-threading, and we can't the problem with multi-threading is is making stuff work with threading in mind and making it more like thread safe and stuff like that so
>
> [Music]
>
> the game does have threading support when when your factory's running like all the machines and all the conveyor belts and something else are updated like simultaneously and they're updated in like batches and stuff like that but they're limited in the way that they're like ordered so like you can't have you know the same belt run two threads separate threads because they're dependent on each other so there's there's a limitation to that, and that's the biggest limitation to to threading support now there's there's a lot more stuff though, tied to like the game than just like your factory and your cpu cycles, one thing for instance is the lights in the game that we've implemented the reason why we're able to add lights to the game was because unreal engine added better threading support for, hr threading, and that made it just like possible to have, multiple lights collide with with each other without it being a big hassle because they can be offloaded better, and that's something there was a way we could talk more to people about these lights only it's funny that you bring that up jace because this way we're actually gonna be releasing a video about that specific topic actually so me and ben, talk about lights and we talk about, some of the optimization systems techniques we're using in that we specifically implemented for update four so stay tuned for that indeed yeah, and i think yeah and that's pretty much like we're constantly looking into more ways to improve performance and threading and stuff like that but we are a little bit limited in the way the the game kind of functions and to some degree we sure are
