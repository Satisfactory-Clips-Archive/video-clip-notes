---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 4)"
date: "2020-10-09"
layout: transcript
topics:
    - "coffee-stainers/dylan"
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 4)
https://www.youtube.com/watch?v=oyHCEA2k1PM

### Topics
* [Coffee Stainers > Dylan](../topics/coffee-stainers/dylan.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> so i'm looking at the bindings now
>
> to see how it's hooked up
>
> this is their static mesh file
>
> that we've imitated you can see here
>
> this is where we've
>
> declared our custom spline
>
> data but i want to see where it's coming
>
> from
>
> okay so yes this is interesting
>
> so we have the f we're actually using
>
> their their mesh proxy
>
> um data type here um
>
> even though this is for the instancing
>
> stuff because it has all the information
>
> that we need and the splendish params
>
> so yeah this and i see here
>
> that they are collapsing everything into
>
> a single
>
> layout field ah
>
> that makes sense so here's what we're
>
> gonna do
>
> we're gonna take this so this is from
>
> the scene splendid scene proxy so if
>
> you're rendering a normal unreal engine
>
> spline
>
> it would be using this to render
>
> that spline mesh but it wouldn't be
>
> instanced
>
> so you could update it on the fly and
>
> everything
>
> go down to blind
>
> so here we have
>
> i'm trying to think if i want to just
>
> nuke these and i think i do
>
> yeah so this is how we used to do it
>
> and i'm going to do this for posterity
>
> it's blind mesh params because that is
>
> in the
>
> ush file should bind to
>
> all of these
>
> yes theoretically
