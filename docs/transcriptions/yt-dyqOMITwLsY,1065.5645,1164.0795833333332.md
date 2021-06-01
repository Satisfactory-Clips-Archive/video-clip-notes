---
title: "May 28th, 2021"
date: "2021-05-28"
layout: transcript
topics: 
    - "technology/graphics"
    - "technology/unreal-engine"
    - "features/transportation/vehicles/factory-cart"
---
# [May 28th, 2021 Dev Vlog: How Lights work in Satisfactory](../2021-05-28.md)
## Q&A: Could you quickly describe what instancing means?
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=1065&end=1165
### Topics
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Features > Transportation > Vehicles > Factory Cart](../topics/features/transportation/vehicles/factory-cart.md)

### Transcript

> could you just like uh quickly uh
> describe like what instancing means
> and like when we talk about that so that
> people are aware of
> what the implication of an instance in a
> game is when you're rendering stuff
> so an instance is you have several way
> of rendering items so you can just say
> like okay this isn't
> rock just render this one single rock
> here
> which is fine you render the rock uh
> with instancing basically you tell like
> okay there are
> 20 rocks here and it can do the task 20
> times in sequence which is really
> fast because it doesn't need to read the
> data again
> gpus are really fast they're really bad
> at switching tasks
> right so it's really fast to render 20
> times the same object in sequence
> knowing it's the same thing then to
> render 20 times the same object without
> knowing it's the same thing in the
> sequence
> right so it essentially batches up the
> things you want to render
> to when you're telling the gpu to render
> them essentially yeah and then
> unreal has their own implementation on
> top of that
> which is an hierarchically uh based
> rendering which does the best of
> both worlds so it has all the instances
> and
> it prepares clusters for themselves uh
> which
> also allow loading and curling and all
> the optimizations normal instances
> cannot do so that's like the best ideal
> case for instancing um we use it on
> absolutely everything yeah
> all the walls are done that way
> everything except for
> this little bastard
