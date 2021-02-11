---
title: "February 11th, 2020 Livestream Snutt & Markus Talk: Adding Multiplayer to a game adds 10x the complexity"
date: "2020-02-11"
layout: transcript
topics:
    - "features/multiplayer"
    - "off-topic/goat-simulator"
    - "technology/unreal-engine"
---
# [February 11th, 2020 Livestream](../2020-02-11.md)
## Snutt & Markus Talk: Adding Multiplayer to a game adds 10x the complexity
https://www.youtube.com/watch?v=jFeV8JA7NXg

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Off-Topic > Goat Simulator](../topics/off-topic/goat-simulator.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> it's so hard to tell because like when
>
> you're doing online stuff
>
> like you need so much more testing for
>
> everything like
>
> adding multiplayer to any game adds so
>
> much more like
>
> 10 times the complexity yeah like
>
> because you don't have time to test
>
> everything
>
> and you have to figure out like how and
>
> and the way we've done is just like
>
> throw it at everyone and see what like
>
> yeah and see what
>
> what bugs surface up yeah and i find it
>
> kind of funny because we've done
>
> multiplayer in
>
> all our games in unreal engine until we
>
> got to go to him later and we said
>
> go let's just get the out
>
> and we got it out in really new time
>
> and the first thing people ask like
>
> where's the multiplayer wait
>
> really i thought i thought for sure
>
> gosim had like multiplayer in
>
> like in the back of your head when you
>
> made that
>
> i think the thing that was in back of
>
> our head is how
>
> can we do get this everything out
>
> as fast as possible and how to get more
>
> stupid in there how do
>
> this stupid idea that i got how do we
>
> present this
>
> to everyone right so just like get
>
> everything out
>
> as soon as soon as possible so
>
> multiplayer in goat sim is like
>
> literally the just add multiplayer to
>
> the single player game or
>
> yeah we had local co-op yeah so you can
>
> play for classic
>
> screen yeah well that actually does save
>
> a bit
>
> because yeah then you need to like
>
> follow the game states and whatnot
>
> yeah which you must have when you do
>
> online yeah but
>
> yeah and i think we tried a multiplayer
>
> session once and
>
> aaron landon3 was like oh you tried to
>
> create this many actor
>
> replication states and like just crashed
>
> and burned and
>
> everything was just shocky because new
>
> physics
>
> all physics textures vibrated on the
>
> spot
>
> and they're like oh so you're vibrating
>
> let's send updates
>
> did you guys have to do like a special
>
> thing for like the physics
>
> in good sim to like be able to sync it
>
> properly no we
>
> didn't do anything more really no like
>
> do you mean
>
> like all like there's so many like
>
> physics objects running like
>
> and syncing that stuff can be really
>
> demanding especially due like ragdoll
>
> and like yeah but
>
> we did our referee in single players we
>
> didn't need to care about okay
>
> like yeah sure we had like a simple
>
> super simple manager that we added that
>
> saved i think
>
> like 20 or 30 milliseconds that just
>
> basically said that
>
> only take the closest uh
>
> like objects that in in your vicinity
>
> and they update in full frame rate and
>
> that was a bit further away
>
> just loading their update rate down and
>
> just let the simulation go but don't
>
> update the visual representation and i
>
> think i threw that together in like
>
> 10 minutes or something the initial
>
> implementation and that saved
>
> yeah 20 milliseconds yeah so
>
> just those super simple things that shop
>
> visual quality
>
> can save so much i think that double o
>
> yeah
>
> i think that got us from yeah 15 enough
>
> pass to
>
> a solid 50 or something that's a good
>
> good one you want to go 60. yeah but we
>
> go
>
> for that we actually need to work a bit
>
