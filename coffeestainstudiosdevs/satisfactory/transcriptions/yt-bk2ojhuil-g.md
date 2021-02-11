---
title: "November 10th, 2020 Livestream Snutt & Jace Talk: Unreal Engine Object Limit"
date: "2020-11-10"
layout: transcript
topics:
    - "features/unplanned-features/mass-building"
    - "technology/unreal-engine"
---
# [November 10th, 2020 Livestream](../2020-11-10.md)
## Snutt & Jace Talk: Unreal Engine Object Limit
https://www.youtube.com/watch?v=bk2ojhuil-g

### Topics
* [Features > Unplanned Features > Mass Building](../topics/features/unplanned-features/mass-building.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> i haven't seen that though yeah so the
>
> only question i have uh i placed one 500
>
> computer and also a 15 000
>
> computer that's crazy and the same
>
> problem occurs the number of principles
>
> uh will it be uh a fix to the amount of
>
> items we have in the save i have
>
> a 100 000 items um and i want to know if
>
> i need to start again i just deal with a
>
> lag okay so first of all there is an
>
> object limit in the game
>
> that has not been put on by us and it's
>
> not bound by hardware it's by the engine
>
> in the recent video with ben he actually
>
> talks about how you can change that
>
> um however that is not supported by us
>
> it's at your own risk because we don't
>
> know for sure
>
> what that is going to do he's observed
>
> more crashes
>
> when people do do that uh so if you go
>
> to our youtube channel i'll link the
>
> video again
>
> yeah it's kind of not recommended
>
> actually by us even
>
> uh yeah and then so also so that's so
>
> that's here's the video
>
> so that's um that object limit as for
>
> the game lagging as you add
>
> uh items like 500 000 items that's gonna
>
> happen
>
> and that's probably gonna always happen
>
> uh
>
> the the difference the thing that we can
>
> do is we can hopefully change the
>
> threshold
>
> so if you're lagging at 500 000 items uh
>
> hopefully we can fix it to a point where
>
> that you get that same amount of lag but
>
> at a million items
>
> but ultimately if you can just build
>
> forever you're going to hit that lag
>
> point at some point yeah um
>
> so yeah we we constantly optimize and
>
> also in that video
>
> uh ben talks about optimization so we're
>
> constantly doing that and things get
>
> better with
>
> every single update they do um it's just
>
> slow it's just incremental and
>
> um yeah so
>
> you will you're going to face the lag
>
> eventually i think there's
>
> i don't think that's something that can
>
> ever be gotten around
>
> removing limit equals gpu uh making a gp
>
> a cooking serve no i don't think so
>
> actually because
>
> the object limit is actually nothing to
>
> do with the gpu it's just sort of like i
>
> don't know
>
> it's memory it's like it's it's the
>
> garbage collector it's a garbage
>
> collector okay
>
> so it's it's memory in general yeah and
>
> and that limit is there
>
> it's it's it's hard set there by default
>
> by epic
>
> yeah uh because like and also
>
> like the the thing you mentioned before
>
> how like we don't exactly know what
>
> happens
>
> if we increase it because you might run
>
> and start running to like seg faults and
>
> like fragmentation issues with the save
>
> file
>
> and stuff like that or like in the game
>
> which can result in your safe while
>
> becoming corrupt and stuff like that so
>
> like it's uh we don't know exactly what
>
> happens uh when people up it
>
> uh what goes on because it's such a
>
> like when epic set that limit they were
>
> like nobody's gonna be able to like
>
> and then we made satisfaction yeah and
>
> then you guys went crazy and built like
>
> amazing [ __ ]
>
> but there's um there's like a lot of
>
> like optimizations that uh ben talks
>
> about even
>
> um to reduce the number of objects
>
> because sometimes an object
>
> an object can be as something as simple
>
> as just a little plane
>
> um and that can count as an object but
>
> sometimes we need that plane
>
> so it's not that the the object is heavy
>
> and expensive on your pc it's just
>
> an object that adds to the counter yeah
>
> um
>
> it's a custom engine yeah so we're gonna
>
> we're gonna work on that now
>
> we're gonna switch to custom download
>
> more ram very good
>
> it's like it's an object it's a data
>
> data memory object that like the engine
>
> keeps track of
>
> and checks references and like make sure
>
> like is this still
>
> live can i use this so yeah it's it's
>
> it's
>
> a little bit more complicated than just
>
> like it's just an item in the game like
>
> uh so like building one constructor for
>
> instance is like
>
> a bunch of objects in the then
>
> memory pool so to speak yep
>
