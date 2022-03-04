---
title: "May 11th, 2021 Livestream Q&A: Is there a fix so the new lights emit shadows?"
date: "2021-05-11"
layout: transcript
topics:
    - "features/buildables/lights"
    - "technology/graphics"
    - "technology/unreal-engine"
    - "technology/unreal-engine/distance-fields"
---
# [May 11th, 2021 Livestream](../2021-05-11.md)
## Q&A: Is there a fix so the new lights emit shadows?
https://www.youtube.com/watch?v=wIvvNslWt78

### Topics
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Distance Fields](../topics/technology/unreal-engine/distance-fields.md)

### Transcript

> is there a fix in the lights emit shadows the new lights do emit shadows, the new lights the the lights that you place are a little bit special because, they in order to save, performance they're pooled and they also use, something that's called, distance fields for shadows, and, there are a few edge cases where they don't work like if particularly if you have like glass and stuff in between, and maybe there are like other cases where maybe they don't show shadows, I really want to make a video about this to explain this a bit more, so I'm probably gonna do that at some point, but like that's that's the reason why you don't see shadows all the time for lights is because they they're like cheat lights they're not like proper proper lights, like the other lights in the game, if I dumb it down projector active special sauce no not really it's it's like it's too much to explain on stream by me I'm also very bad at explaining this but like this is this is, it's a very odd system to some degree it was actually made for paragon fun fact so if it weren't for paragon we wouldn't have licensed satisfactory one of the good benefits that epic make games, while working on their engine is that they actually like find like use cases and they're like oh we need to implement this what's paragon oh no now I feel so sad paragon was a, a pvp like third person moba that epic made, they made this while they started making, fortnight and they were developing these two games in like in in synchronous, and paragon was actually pretty fun it was like it was the only mob I actually got into, but the yeah it had pacing issues I actually enjoyed the pacing issues to a certain degree because, like when you actually had a good match it was it was a really good match but the thing was that it was so hard finding a good match so like it got a bit tedious but they they they they were in the pretty good track I'd say but then they they ditched development, and they and they refunded everyone who bought stuff for paragon, but I really enjoyed it but one of the really good things about paragon there came a lot of good techniques was implemented in paragon that were then integrated into unreal engine one of which was near field near distance fields that they used for shadows on their characters that we then used for lights and shadows, and buildings etc so, they did a bunch of other cool and a bunch of vfx work were also done perennial engine but yeah good stuff now it's just paragon, sorry no it's just fortnite
