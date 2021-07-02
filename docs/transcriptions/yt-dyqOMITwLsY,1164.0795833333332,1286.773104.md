---
title: "May 28th, 2021 - Snutt & Ben Talk: Holograms now use Stencils"
date: "2021-05-28"
layout: transcript
topics: 
    - "technology/user-interface/holograms"
    - "technology/graphics"
    - "features/save-system"
---
# [May 28th, 2021 Dev Vlog: How Lights work in Satisfactory](../2021-05-28.md)
## Snutt & Ben Talk: Holograms now use Stencils
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=1164&end=1287
### Topics
* [Technology > User Interface > Holograms](../topics/technology/user-interface/holograms.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Features > Save System](../topics/features/save-system.md)

### Transcript

> stencils instead of the mesh itself
> so if we would show a stencil
> [Music]
> and what is a stencil this is a stencil
> so we are allowed to
> write an id a bit to a separate buffer
> and we can read that buffer in
> post-processing and based on that buffer
> we can um apply certain effects
> so if i would change to two three four
> five here we go we have different ids
> and if we go back into the game view
> there we go and then we can
> apply an outline to it with that effect
> magic dismantle effect so now you can
> dismantle this rock
> totally not a lie but this is how we can
> apply the hologram to this rock for
> example
> so essentially what you're doing when
> you're doing the hologram effect now
> instead is you're kind of drawing
> on top of the screen sort of with effect
> rather than it being like how everything
> else is rendered in the game where it's
> all like word space and it's
> yeah yeah so technically it's like
> putting on shades
> for this specific object right and i
> guess the limitation of doing it that
> way means that you can't have
> transparency
> on that object anymore because you're
> setting the the the frame is already
> drawn
> and you're drawing on top of the frame
> so it's impossible for you to know like
> what's behind
> something that's already been rendered
> that's the problem with it
> but the trade-off was so great
> because accidentally it also improved
> saving times
> which was not the intention but
> still could win i understand why after
> the fact but i didn't think about it
> when we were doing it let's say that way
> um and also one we'll take it you know
> what we'll take it okay
> we'll take any benefit that we can get
