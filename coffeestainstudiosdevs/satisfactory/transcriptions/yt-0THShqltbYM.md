---
title: "October 9th, 2020 Livestream Dylan Talk: Working on the Replication Graph"
date: "2020-10-09"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "features/multiplayer"
    - "technology/unreal-engine"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Working on the Replication Graph
https://www.youtube.com/watch?v=0THShqltbYM

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> concordantly visa and like in those
> 
> different aspects too
> 
> so i had earlier in the stream i
> 
> mentioned that i've been working on
> 
> the networking stuff which is actually
> 
> in this context would be the replication
> 
> graph um
> 
> so i had updated that to 425
> 
> before so we could have the replication
> 
> graph because that that has a lot of bug
> 
> fixes
> 
> um and when i was doing that implemented
> 
> some
> 
> nice optimizations there so like
> 
> that won't show up on a profiler as a
> 
> performance issue
> 
> right but when you're running a server
> 
> um
> 
> that's a whole separate thing so there's
> 
> a lot of different areas to optimize
> 
> unfortunately yeah but those those
> 
> will be coming in uh hopefully soon tm
> 
> but we've been working on a lot of
> 
> things besides behind the scenes oops
> 
> kind of the state of affairs so there's
> 
> good stuff talk about
> 
> the uh like the replication system that
> 
> you're working on
> 
> uh let's see yeah um and the major
> 
> changes do you have anything you can
> 
> show
> 
> um before we wrap up actually
> 
> i wish i did i have three branches yeah
> 
> let me see
> 
> if i have a image here
> 
> i don't want this to show on stream
> 
> if it's not uh
> 
> let me see real quick
> 
> whoa my god whoa look at that oh i wish
> 
> you could see the other monitor right
> 
> now chad but that is amazing
> 
> i can't believe you have that on your
> 
> computer like that done
> 
> that is wild stuff right yeah i know
> 
> dude i'm
> 
> my mind is blown for some reason this
> 
> file is not
> 
> there we go great pain yeah so this is
> 
> this is a graph that i know this is a
> 
> optimization thing
> 
> that's oh yeah this is um
> 
> and this feature isn't fully complete
> 
> but what i'm essentially doing here this
> 
> is the way it
> 
> works not now no this is not now
> 
> but you can see a bunch of
> 
> the replication system works like
> 
> range checks basically and what i'm
> 
> implementing is a way that
> 
> belts will only send their network data
> 
> when they're actually in the view
> 
> frustum so
> 
> in this case you can see the i've set up
> 
> a grid
> 
> and the green indicates that it's a
> 
> high replication rate you can see here
> 
> it says frames till that basically means
> 
> it's replicating every frame which means
> 
> it's sending data every frame
> 
> but in the current way and the default
> 
> replication system
> 
> it doesn't matter which way the player
> 
> is looking so these black boxes back
> 
> here which you can see it's
> 
> period 60 which means uh it's never
> 
> going to replicate
> 
> or send it send its data these would
> 
> also be sending data in the current
> 
> setup
> 
> so if i look the opposite direction you
> 
> can see everything behind me is no
> 
> longer replicating
> 
> and this like there's a lot of more data
> 
> but
> 
> the key takeaway here is this is what it
> 
> would be like now
> 
> but it would stay that way no matter
> 
> which way i was looking but in this
> 
> it dips down a lot so we're going down
> 
> from 25 kilobytes per second
> 
> all the way down to 10 10
> 
> and this is a huge these are densely
> 
> layered conveyors
> 
> and lifts i actually got this uh file
> 
> from ben because he was testing the
> 
> instancing on them i think
> 
> um yeah so this is one of the
> 
> optimizations going into the rip graph
> 
> for just conveyor belts because they're
> 
> kind of unique
> 
> so good things to come
> 
> yo will that fix the no no i mean
> 
> it'll a lot of issues do come from set
> 
> over saturation of bandwidth
> 
> yeah so by doing these improvements we
> 
> can
> 
> uh smooth out the rough parts
> 
> yeah i just i think i just want to show
> 
> this because
> 
> green is good and you know green's good
> 
> loose like okay
> 
> you know red is like that's bad orange
> 
> you know yellow it's okay
> 
> bad it was is actually pretty
> 
> substantial improvements to the
> 
> replication but we won't see this
> 
> improvement in a long time
> 
> it'll be it'll be a little bit it's i
> 
> think this
> 
> is going to come with the engine upgrade
> 
> whenever that
> 
> goes and there's going to be so many
> 
> other issues that you're not going to be
> 
> able to like
> 
> probably but so
> 
> we're we're working on it
> 
> we hear you yeah
> 
> um but i think it'd be good stuff
> 
> there's a lot of stuff going on right
> 
> now
> 
> at the same time at the studio so it's
> 
> kind of hard to uh
> 
> to uh explain it but uh there's there's
> 
> a
> 
> lot of work that's happening in the
> 
> background pen fighter i could
> 
> read your text all day
> 
> that's what i'm saying yeah
> 
> and lack of bandwidth was one of the
> 
> yeah that's a persistent the
> 
> over saturation of bandwidth is leads to
> 
> a lot of
> 
> issues
> 
> and the the problem with the fps why
> 
> does it take so long to improve fps
> 
> is because while we're improving the fps
> 
> you guys keep making bigger bases so cut
> 
> it out
> 
> well it's okay because we have the uh
> 
> the object limit
> 
> to stop yeah that's like the hard limit
> 
> like all right just take it easy
> 
> but that limit though i some of the
> 
> saves that i've loaded and i've been
> 
> profiling on and testing
> 
> it's uh they're so insane
> 
> i mean you guys are amazing but it's
> 
> ridiculous like if you asked me like
> 
> what
> 
> what's the biggest base somebody's gonna
> 
> make like it probably would have been
> 
> like a half or fourth the size of some
> 
> of the ones we're getting
> 
> insane it's amazing
> 
> all right
> 
