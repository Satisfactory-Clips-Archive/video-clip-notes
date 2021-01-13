---
title: "Q&A: How did you guys optimise the game so much?"
date: "2019-03-09"
layout: transcript
topics:
    - "technology/graphics"
---
# [March 9th, 2019 Livestream](../2019-03-09.md)
## Q&A: How did you guys optimise the game so much?
https://www.youtube.com/watch?v=nRCmJo-Wh9s
> correct how did you guys optimize the
> 
> game so much that gtx 1050 can play
> 
> high ultra settings with great
> 
> difficulty there's like some
> 
> like obviously there's like programmers
> 
> that can optimize stuff but then also
> 
> like
> 
> there's a lot of things our artists can
> 
> do as well and so everyone has just been
> 
> working their ass off completely
> 
> that's uh simon's dig or yeah actually
> 
> i work a lot of optimization and kafka
> 
> or
> 
> like the news programmer there like he's
> 
> done some really cool
> 
> stuff with all the buildings so like for
> 
> example if i build one of the
> 
> constructors
> 
> or let's say i built 50 constructors we
> 
> have instanced one of them so like
> 
> yeah they're only rendered like this
> 
> this constructor is supposed to be here
> 
> and you just yeah it's one like one drug
> 
> so
> 
> you can draw all 50 constructors in one
> 
> call yeah exactly
> 
> but we also have like it's divided up
> 
> the skeletal mesh as well so the
> 
> the moving part is a separate object on
> 
> the buildings
> 
> okay so there's like more stuff we can
> 
> do there which
> 
> probably gonna come in some stuff for
> 
> relaxes i hope
> 
> like this it's gonna come in eventually
> 
> but yeah
> 
> and we did some we did some tricky [ __ ]
> 
> with the conveyor belts as well right
> 
> g2 is the guy who made the trains as
> 
> well uh it's yeah g2 and stack has done
> 
> like marcus
> 
> if you guys have seen him on discord
> 
> marcus has done a ton of optimization on
> 
> the conveyor belts
> 
> recently that just upped the
> 
> the the performance crazy
> 
> yeah like like back in the day the way
> 
> that we did the like drew the conveyor
> 
> belts they were piece by piece right
> 
> like
> 
> it wasn't really it wasn't even like a
> 
> spline is that right or
> 
> yeah it was it was still a spline but
> 
> all the separate like
> 
> pieces off this like every way can i i
> 
> can actually show on
> 
> screen if i can
> 
> like because it was like there was still
> 
> multiple pieces on one spline right it
> 
> makes up like
> 
> oh yeah i can't show it okay so so yeah
> 
> so like every time you place down a
> 
> conveyor belt and connected it like so
> 
> this would be one piece
> 
> um that's one spline but on the spline
> 
> there are
> 
> separate meshes for everything exactly
> 
> and then if you
> 
> if you did this for a ton like a whole
> 
> bunch of conveyor belts that's a lot of
> 
> draw calls
> 
> it entire factory and you look at it
> 
> yeah so now it's
> 
> right now it's like one draw call purse
> 
> line yeah like so if you
> 
> if you have a conveyor pole i think it's
> 
> a new new draw call
> 
> like of every conveyor belt like exactly
> 
> exactly
> 
> and that's the next thing to do is to
> 
> have so that all the splines
> 
> like all the connections being kind of
> 
> labels is just one draw call instead of
> 
> first per pole so to speak so there's
> 
> still stuff to do
> 
> that will also improve it hey [ __ ]
> 
