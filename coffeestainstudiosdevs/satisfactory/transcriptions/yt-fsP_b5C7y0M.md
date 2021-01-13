---
title: "December 8th, 2020 Livestream Snutt Talk: Lights on Buildings"
date: "2020-12-08"
layout: transcript
topics:
    - "technology/graphics"
    - "features/buildings"
---
# [December 8th, 2020 Livestream](../2020-12-08.md)
## Snutt Talk: Lights on Buildings
https://www.youtube.com/watch?v=fsP_b5C7y0M
> i want to comment on one thing though
> 
> that i've seen some people comment on is
> 
> the fact that
> 
> there are lights on these buildings um
> 
> and it's this is true because these
> 
> lights on these buildings
> 
> are uh not emissive lights so on the
> 
> we've struck a balance on the current
> 
> build there are certain
> 
> buildings that have actual lights on
> 
> them i think the workbench is one of
> 
> them
> 
> that has like one light on it um so in
> 
> this early version a lot of stuff did
> 
> have
> 
> actual lights on them like all the
> 
> buildings had lights the the
> 
> power pole geez power pole did have
> 
> lights on them and it's just something
> 
> that i guess we realized that
> 
> as you're building like the frame rate
> 
> just suffers because of that because of
> 
> the
> 
> extra calculations that are needed to to
> 
> have
> 
> that many like dynamic lighting in the
> 
> game so we scrapped it like we
> 
> removed it because we noticed that the
> 
> game suffered for it
> 
> um and if we were to reintroduce it we'd
> 
> have to figure out a
> 
> better system for it um than the way
> 
> this was implemented because
> 
> when people say like you haven't even
> 
> tried lights we have tried lights like
> 
> the yeah it's it's not as if it's not as
> 
> if
> 
> lights are a hard thing to prototype
> 
> lights are built into every video uh
> 
> game engine you just drag and drop them
> 
> you get a light it's easy
> 
> they're easy to make but but it's it's
> 
> one thing to to
> 
> have the ability to put lights down it's
> 
> another thing to sustain it as a
> 
> gameplay feature
> 
> yeah um and that's where things get hard
> 
> especially in a game like this
> 
> and some lights on the current buildings
> 
> like i think
> 
> on on like smelters and miners and stuff
> 
> like that the lights that you see in the
> 
> game right now
> 
> are kind of like fake lights they're
> 
> baked into the materials so that
> 
> they will do this kind of effect um and
> 
> then there's like screen space
> 
> something where like when you're looking
> 
> around it will affect the things around
> 
> it but it's not actually
> 
> so there's like a bunch of tricks we've
> 
> used to
> 
> kind of like fake that effect
> 
> and sometimes like on the workbench i
> 
> believe i actually have
> 
> like actually have one light on it but
> 
> you don't build
> 
> like 50 000 workbenches you build a few
> 
> um so they they don't suffer that much
> 
> but
> 
> for power poles for instance you build a
> 
> lot of power poles so having one light
> 
> on each power pole like had a huge
> 
> um effect on on rendering
> 
> because of that because of the way
> 
> people build power poles and the way
> 
> they're
> 
> used in the game
> 
