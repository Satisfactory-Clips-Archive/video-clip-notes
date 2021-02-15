---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 9)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 9)
https://www.youtube.com/watch?v=pj50SOLT17Q

### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> okay so
>
> i think i have these bound correctly if
>
> i'm
>
> not filling myself
>
> so i need to
>
> modify this so before we had our uh
>
> parameter layouts here
>
> and this is key this will if these don't
>
> match up it will
>
> crash very very very badly
>
> shader see
>
> i'll show you i think it's so we're our
>
> parameter our spline
>
> data is an array and i think there's a
>
> custom macro for that
>
> parameter type so i'm going to check out
>
> the
>
> sheet of parampar sampler array
>
> uh feels feels good
>
> a sampler though no i just want a
>
> parameter
>
> ah
>
> got a that's an srv though i don't want
>
> an srv
>
> there we go shader parameter right
>
> it takes a type the actual
>
> member and then the length i'm just
>
> going to take there's
>
> this comment thank you epic for putting
>
> that comment there
>
> and our types are
>
> effector force
>
> which we could see in the uh where'd it
>
> go
>
> the ush file did i close that
>
> text factory dot there it is
>
> because we have a yeah float4 spline
>
> params 10.
>
> so we are going to do effector
>
> 4 possibly
>
> it was
>
> mesh air spline
>
> mesh
>
> anything's it's just spline params
>
> is that any hits for this
>
> yep okay cool it's one mesh params
>
> and it wasn't length eight it was like
>
> ten
>
> so this is our custom vertex buffer
>
> which should still be good and then we
>
> have this new
>
> parameter arrays rather than passing in
>
> single floats we're passing in
>
> a whole array here
>
> this comment still makes me chuckle this
>
> is done correctly i don't know i guess
>
> we'll find out
>
> hold on to your butts
>
> i'm going to try to run this to see what
>
> it complains about
>
> i mean i see to see it work and be
>
> perfect
