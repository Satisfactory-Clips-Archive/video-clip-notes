---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 10)"
date: "2020-10-09"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 10)
https://www.youtube.com/watch?v=0VtsjQsFzZU

### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)

### Transcript

> like that's interesting yeah
> 
> and then we never got around to doing
> 
> implementing that and then uh yeah
> 
> i've seen this history you've seen this
> 
> yeah that's kind of weird
> 
> so that is this okay that's like that's
> 
> this
> 
> mesh without the spline doing anything
> 
> on it yeah
> 
> and it wasn't it wasn't there before
> 
> why is it backwards well i'm guessing
> 
> that would be the default
> 
> like if the origin it is so the world
> 
> position and
> 
> tangent and stuff is all yeah because if
> 
> you aim at the other one the other left
> 
> side of that
> 
> it should be the same position but no
> 
> it's going to be on the other one
> 
> know what i mean on the other one like
> 
> yeah yeah
> 
> because that's going forward exactly
> 
> yeah
> 
> that's what i mean yeah so why does it
> 
> only show when i dismantle
> 
> because the dismantle actually applies
> 
> the material on
> 
> the the mesh
> 
> yeah that is oh no it's just always
> 
> world origin
> 
> okay that looks like because this is so
> 
> everyone knows this is zero zero
> 
> just something to remember yeah so
> 
> that's the world that's just default
> 
> transform
> 
> okay isn't it relative
> 
> no because it was it's always facing the
> 
> same because zero zero is
> 
> is a bit right to where you are well
> 
> it's its position is relative but it's
> 
> i'm saying it's a rotation
> 
> okay it's basically just using uh none
> 
> okay i'm going to take a look at the ush
> 
> here
> 
> ish
> 
> which i apparently only have on one of
> 
> my desktops if you're
> 
> wondering why i'm not finding it
> 
> sometimes
> 
> okay what's trying to stand on one like
> 
> the the conveyor belts do work
> 
> stan they are there and they will
> 
> transport items they just don't render
> 
> yeah so i'm trying to fix
> 
> the rendering portion of it
> 
> factory get world position
> 
> is this the one we modified no
> 
> we want instance position
> 
> oh wait wait wait a minute so this is
> 
> under death pass only
> 
> we're doing something different here
> 
> bp material effect conveyor build
> 
> reports no material is set
> 
> uh i don't think that's tied to this
> 
> issue no actually
> 
> yeah i've noticed that that is something
> 
> to do with the order of
> 
> events with our spline meshes their
> 
> build effect is totally different from
> 
> the
> 
> standard build effect and it i think it
> 
> creates an actor
> 
> which creates a bunch of components so i
> 
> think there's a frame where it's
> 
> creating the actor that's going to
> 
> build do the build effect and so it's
> 
> missing for that frame
> 
> we should fix that i think that's been
> 
> there
> 
> it's i think it's been there a long time
> 
> for a long time
> 
> i think that's on poles as well get the
> 
> same error
> 
> okay calc slice transform
> 
