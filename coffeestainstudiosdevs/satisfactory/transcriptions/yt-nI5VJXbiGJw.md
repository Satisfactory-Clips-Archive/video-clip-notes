---
title: "October 9th, 2020 Livestream Q&A: How are the Fluids calculated in the Pipe?"
date: "2020-10-09"
layout: transcript
topics:
    - "features/fluids"
    - "features/fluids/pipes"
    - "off-topic/factorio"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Q&A: How are the Fluids calculated in the Pipe?
https://www.youtube.com/watch?v=nI5VJXbiGJw

### Topics
* [Features > Fluids](../topics/features/fluids.md)
* [Features > Fluids > Pipes](../topics/features/fluids/pipes.md)
* [Off-Topic > Factorio](../topics/off-topic/factorio.md)

### Transcript

> how are the fluids calculated in the
>
> pipe do you have time for that dylan
>
> well wow that's a big question
>
> um we have every
>
> everything that's part of the simulation
>
> has a fluid box which is just a very
>
> small struct
>
> we compare the pressure differences
>
> which is based on the height
>
> and volume of each different box
>
> and propagates the pressure
>
> in a i think it's three passes now
>
> in different passes and create pressure
>
> groups so we know the top of the water
>
> so we can have the water push things
>
> down
>
> and we combine groups and ultimately
>
> derive the flow
>
> between the boxes from all the
>
> precalculated pressures
>
> and that is that that should be pretty
>
> obvious right sounds simple enough i
>
> don't understand why people have such a
>
> hard time getting that
>
> basically it's they're just simple boxes
>
> that have water in them or like a liquid
>
> and we use the volume the height and its
>
> previous
>
> flow rate and the
>
> pressure so like a pump adds pressure
>
> and so like
>
> when it compares the pipe that it's
>
> attached to it would say
>
> i i have this much pressure you have
>
> none okay i'm going to move liquid this
>
> is very laymen but move
>
> liquid from me into you because you're a
>
> low pressure front
>
> essentially and then it moves down
>
> the line but we have to do multiple
>
> passes to get it so that
>
> they can consider all sides
>
> um and it plans for different liquids to
>
> act differently i think they do
>
> they we they do kinda it's not that
>
> noticeable
>
> because you can't see them the like we
>
> do have viscosity properties
>
> on them um if this if they haven't
>
> changed this if design hasn't changed
>
> this but
>
> um if you it's weird when you initially
>
> hook up
>
> like to an oil line you will see that
>
> the oil takes longer
>
> to get to the end of the line if you did
>
> it identically with like a water pump
>
> it would take longer to get to the end
>
> of the long chain
>
> but yeah yes mostly it doesn't have a
>
> big
>
> impact on gameplay
>
> so it's a bit like factoria's pipe
>
> system with a twist and
>
> yes factoria's pipe system is a big
>
> inspiration to that actually
>
> yes or like at least the initial one
>
> well they
>
> i think we uh started by reading their
>
> dev blogs about it too because they had
>
> a lot of
>
> like this didn't work this did so we
>
> wanted to
>
> see save a lot of work like believe it
>
> or not neither one of us had ever
>
> written
>
> a water pipe simulation before yeah it's
>
> not really something that
>
> comes up often but it's like where to
>
> begin it was actually it was a ton of
>
> fun
>
> working with the g2 on that yes i guess
>
> the main difference is that we've added
>
> another
>
> uh dimension to it yeah that
>
> and that has caused a lot of a lot of
>
> our issues stemmed from that too
>
> yeah yeah having that verticality
