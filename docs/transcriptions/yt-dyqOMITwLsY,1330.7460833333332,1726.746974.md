---
title: "May 28th, 2021"
date: "2021-05-28"
layout: transcript
topics: 
    - "technology/unreal-engine"
    - "satisfactory-updates/released/satisfactory-update-4"
    - "features/buildables/conveyor-belts"
    - "technology/graphics"
---
# [May 28th, 2021 Dev Vlog: How Lights work in Satisfactory](../2021-05-28.md)
## Snutt & Ben Talk: Impact of the Engine Upgrade on Conveyor Belt performance
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=1330&end=1727
### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Satisfactory Updates > Released > Satisfactory Update 4](../topics/satisfactory-updates/released/satisfactory-update-4.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> should we move on to the next thing
> we're going to the big bus
> the big bus this one doesn't mess around
> the big bus so this is my
> beautiful test case for oh and realistic
> conveyor belt case i recognize let's
> talk about conveyor belts
> um with the engine upgrade we faced the
> same
> issue that we got with the loading the
> conveyor belts got way more expensive to
> render
> i kind of figured out why but we cannot
> change it because it's like in the core
> of the rendering system of
> unreal which is such a black box to me
> that it's like
> can't touch this so we decided to find
> our way around it
> um let's disable the average heifer to
> begin with
> and go to the old system of whereabouts
> so this is the old conveyor belt system
> that's still
> accessible to everybody you can see the
> beautiful
> colors just to turn like are yellow
> even on my shitty screen share what i
> don't even get like a
> proper frame rate i i'm like noticing
> the difference here
> yep um also a lot of items look like
> they're moving backwards
> uh thanks to the framerate but we
> figured out that
> updating instances became more expensive
> sadly enough
> i assume it has to do with gpu
> bandwidth and threading and all that
> stuff that got improved so they had to
> cut corners elsewhere i assume
> i still didn't fully figure out but
> we'll see so our solution to that
> is what if we don't update the instances
> so that was the solution in the end so
> what we do instead
> we render the positions of the items
> on a texture and in the material
> we read where those items are
> so if i can find that subsystem
> here we can see how it looks like if it
> doesn't crash
> please okay so here we see all the items
> in the scene right now
> on the texture what a weird way to
> present that
> or look at it so technically it's
> it's just an array to the array of items
> um
> it's a floating texture which is not
> representable in colors so that's why it
> looks super
> weird every row is an
> item at least every three rows is an
> item because the first
> id is the lot zero then lot one lot
> and then the last slot
> and then we store xyz of this of course
> and the alpha is just there
> interesting and we do the same for the
> orientation
> which is looking even more weird yeah
> because this is
> this is readable but it's not because
> we're using quaternions
> yeah um i don't want to go into
> quaternions
> because nobody wants to
> because they're weird yeah uh they're
> super weird it's like
> let's represent an orientation with four
> numbers
> yep yeah uh and also they are going from
> negative one to positive
> one to make it even more obvious what it
> is
> so yeah we're using quaternions for that
> the reason for that it's
> easier to do it in the shader you can
> just multiply
> by quaternion and they get the right
> offset
> instead of doing xyz rotation then you
> have to do the right order and
> yeah right do you get like precision
> issues
> being that you render it to a buffer or
> does it actually like
> not really matter surprisingly i haven't
> noticed anything yet because it's in
> 32-bit buffer per channel yeah
> so it's quite memory expensive but it's
> again it's cheaper than having and and
> okay just just do a few step back
> we used to have a instance component
> per unique item per conveyor belt
> right let it sink in so if you would
> have five different items on the long
> conveyor belt you have five unique
> components
> in the end that was more of a memory
> sink
> than having a big ass texture
> or 32 uh 32 bits per channel
> uh that was just cheaper like in the end
> this is taking 1100 kilobytes to render
> uh so that that's pretty cheap
> how does it scale when you have like 10
> times as many conveyor belts as you have
> in this scene versus like
> you know a million millions of creative
> ones or whatever it has a cutoff point
> at one point it just doesn't render the
> last lot right i'm not sure if we can
> get there
> that's pretty far away yeah here you can
> see that the purple line and the purple
> fade away it's really difficult to see
> but
> it's quite far you can almost not see
> the items anymore uh
> and there is consideration to make like
> a far distant version
> for far distance only but if we get
> there
> yeah and um the biggest cost of this
> system is on the cpu right now
> which is costing this scene is costing
> 1.1 milliseconds to
> do to render all these items and update
> it because it needs to run on the game
> thread sadly enough
> okay it was fully threaded
> it was fully working and then i pushed
> it out and everybody in the studio was
> crashing
> i was like but it works on my machine
> so one of those classic ones like with
> threading that works in your machine and
> then other people
> yeah except for only me and dylan were
> were running it and everybody else was
> crashing so i was like
> yay well obviously you and dylan were
> doing something much better than
> everyone else
> of course obviously um so yeah i had to
> strip it out and have to
> add that back one day cool so yeah those
> those are the items
> they are nice so i guess there's still
> like a couple of
> uh i've seen some people say that
> there's still a couple of parts that
> haven't
> moved over to like the new system um if
> you do find these
> make sure to go to our qa site questions
> outside of factorygame.com
> and let us know and that goes for all