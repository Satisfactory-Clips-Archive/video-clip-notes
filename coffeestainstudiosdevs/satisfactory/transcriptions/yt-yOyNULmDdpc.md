---
title: "May 19th, 2020 Livestream Snutt & Gafgar Talk: Optimisation passes"
date: "2020-05-19"
layout: transcript
topics:
    - "technology/unreal-engine"
---
# [May 19th, 2020 Livestream](../2020-05-19.md)
## Snutt & Gafgar Talk: Optimisation passes
https://www.youtube.com/watch?v=yOyNULmDdpc

### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> we'll see yeah it's it's like when when we do this optimization passes we often like we've had these rounds of like you find the most the the lowest hanging fruit so to speak of like this is this is a simple thing we can do that will gain a lot of performance budget from or whatever uh and we haven't really had that for a long time there's like one thing i know of and that's the how we send foliage through the network i i know a few others you want to list them you want to shame people on online stream like like one there was a few things that i really want to fix for example every uh wire a power line wire uh is currently a separate draw call unless someone changed something recently that i'm not aware of but they are one separate draw call and they're kind of simple mesh but that's just because the length and their bend and so on we it's it's hard that wasn't support to put into instancing before but we could do it now uh it but in the end there's not a lot of time spent on the frame on the wires but it's still kind of significant right conveyors that's the one thing i was also thinking of yeah the way because we have done optimization of how how where we chunk the render calls to them but there's still more we can do to that yeah so it's like we the engine doesn't in in base like engine doesn't support uh instanced it's called when you draw a lot of meshes at the same time uh spline meshes and the commerce or splines um so we had to add that so we are drawing instant splines uh but the issue is then handling load with that it's not optimal right now and it also means that we still just draw one conveyor at a time we could actually group conveyors into one draw call and make that cheaper as well and then there are items on top of the of the the conveyors you can only currently draw all the items on one conveyor in one draw call but you can actually group neighboring conveyors items into one draw call if you do some more cpu logic before and there's a bunch of stuff that i feel like hey it's work but i think we get a lot of a lot from it yeah um i was gonna say yeah no yeah there's still like there's always stuff to do um there's constantly like solutions that we feel like are we could could do better and there are things that we want to improve on at some point uh but that's the the problem with like producing in the game this way that we are like having it on early access like we have to work on many things at the same time kind of yeah
