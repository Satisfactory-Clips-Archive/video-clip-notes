---
title: "January 19th, 2021 Livestream Snutt Talk: Engine Upgrade - Network tweaks"
date: "2021-01-19"
layout: transcript
topics:
    - "features/multiplayer"
    - "technology/unreal-engine"
---
# [January 19th, 2021 Livestream](../2021-01-19.md)
## Snutt Talk: Engine Upgrade - Network tweaks
https://www.youtube.com/watch?v=cjQzivCIdIU

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> and so what we've increased is the maximum bandwidth for network quality settings so it means that if you have the game set to ultra right now, that will increase like that setting you've been able to like manually do this, but now we're kind of like changing the way the game sets it, and what does that mean that means that, all our network settings will have a higher amount of bandwidth, as you're playing so you know normal whatever to call i can't remember the names of them but like essentially the amount of of network data that's transported, in each, like per second i guess, because it's count it's it's, it is, defined in hertz, it will increase a little bit so if you're playing if you've set the game to ultra right now and you start to run into issues try backing down a step not network tick, or be it i think we increased that too actually i know that i think about it or maybe that's something that's coming but i think i think the game is running at 20 ticks per second or 20 hertz for i think we're up to 30 now or 40. i can't remember i think that's improv but it's not in the patch notes i'm not sure if it actually came in this setting, 20 tick on high setting yeah no it's it's always been 20 regardless of what setting you've had on, and we'll see what happens because the thing with that is that if you have like big basis you might get worse network performance because of that so we'll see kind of based on your feedback what happens there if we if we decide to go with it or not or maybe we didn't do it because it's not in the patch notes so that that was something that we looked into anyway, and there's been a general bandwidth reduction in the game in general so we've optimized like bandwidth consumption for hud and localization for the replication graph which is the underlying replication layer, and then inventory replication and like a lot of minor replication changes so it's essentially like we've we've done some optimization on networking in general
