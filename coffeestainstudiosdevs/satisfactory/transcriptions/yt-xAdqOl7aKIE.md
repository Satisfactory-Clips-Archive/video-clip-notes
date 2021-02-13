---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 9)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 9)
https://www.youtube.com/watch?v=xAdqOl7aKIE

### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> okay so this is
>
> interesting yeah i don't want any of
>
> this
>
> let's take a look here return variant
>
> transform
>
> local world so the things that have
>
> changed since we changed the
>
> spline params i have to make sure that
>
> they're all lining up
>
> okay and before
>
> [Music]
>
> before i'm in the 423 version i won't do
>
> the compare now but we actually had a
>
> custom
>
> implementation for these two and i'm
>
> worried that we're going to have to
>
> revert to that
>
> um but it was basically we called one
>
> function which would call
>
> their code if it was their splines and
>
> would call our code if it was our
>
> splines but
>
> now that we're using their data we
>
> thought it would be best to
>
> try to merge the two and this is
>
> essentially just
>
> zeroing everything out that we don't use
>
> for the instancing
>
> that comes with the data
>
> so
>
> um nice thing is i think
>
> let me see i'm googling something real
>
> quick
>
> i wonder if this will like uh
>
> break everything
>
> i think there's a console command for
>
> i've modified the ush file
>
> and i think i can read file but i can't
>
> remember if there is
>
> oh yes the urge file does anyone in chat
>
> now if you can
>
> what was the thing i want to recompile
>
> because i've modified the
>
> the uh local vertex factory.ush and i
>
> think i can
>
> force that while running but
>
> i don't i think i've just yeah i don't
>
> know i mean i can restart the editor but
>
> yeah that's what i do
>
> hi alert
>
> okay uh but it might also recompile
>
> everything
>
> yeah i'm just gonna restart i have done
>
> this now that i think about it
>
> have you now yeah because i did custom
>
> rendering pipeline stuff once and uh if
>
> you don't do that then
>
> it takes years
>
> it's like isn't there like recompile
>
> shader command something something
>
> um well you can't check now because you
>
> close the editor i guess
>
> yeah let me just there's a force
>
> something force recompile yeah i'm
>
> restart i'm just gonna restart the other
>
> see if this helps at all
>
> do
