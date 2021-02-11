---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 3)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 3)
https://www.youtube.com/watch?v=JrWLEvJRhHM

### Topics
* [Technology](../topics/technology.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> see this oh this is another thing
> 
> that is so this is the way we used to
> 
> that we've been doing it
> 
> we actually had to change to layout
> 
> fields these used to be
> 
> declared specifically i think this is a
> 
> change in 425 it might have been 424
> 
> and we had to have a custom serialized
> 
> function which best in all these
> 
> parameters
> 
> but they've flattened the structure of
> 
> everything and so it
> 
> can basically it has to do less cpu
> 
> calculations
> 
> it can it knows the size and that's what
> 
> this
> 
> uh macro is doing a little bit this is a
> 
> there's my cat this is a little weird to
> 
> me too because this
> 
> is actually from their code and then it
> 
> says it's a legacy macro
> 
> declaration i'm going to leave it but
> 
> i wonder if it will switch in the future
> 
> to using that and what this is doing is
> 
> stating the type and matching to a
> 
> actual
> 
> parameter which we saw below
> 
> and this is all like new as of
> 
> three days to me so bear with me a
> 
> little bit
> 
> because i hadn't looked at these macros
> 
> before
> 
> so let's see the other
> 
> interesting thing that i'm going to do
> 
> now is i'm curious
> 
> about the scene mesh proxy
> 
> so unreal does have
> 
> spline mesh components and to render
> 
> them
> 
> it has its own method of doing that but
> 
> we can't use that because it's not
> 
> instance
> 
> which means it would run terribly slow
> 
> and
> 
> basically ruin everyone's factories
> 
> so we have to
> 
> uh we have to make sure they're
> 
> instanced basically and that's what i'm
> 
> doing
> 
