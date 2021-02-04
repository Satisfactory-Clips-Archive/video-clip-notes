---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 11)"
date: "2020-10-09"
layout: transcript
topics:
    - "coffee-stainers/dylan"
    - "features/buildables/conveyor-belts"
    - "features/fluids/pipes"
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 11)
https://www.youtube.com/watch?v=fJRZSb0W8mQ

### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)
* [Coffee Stainers > Dylan](../topics/coffee-stainers/dylan.md)
* [Features > Fluids > Pipes](../topics/features/fluids/pipes.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> all right let's see what this does now
> 
> because those those things i added were
> 
> definitely
> 
> not being calculated so let's see
> 
> come on vertices oh
> 
> oh i've never been so happy to see a
> 
> stupid spline in my entire life
> 
> hello mr conveyor belt look at that oh
> 
> you even got it right oh nice i am like
> 
> 10 seconds behind with the rest of the
> 
> stream so
> 
> hey yeah
> 
> you did it goku
> 
> holy crap when i set out to actually get
> 
> this to render on stream i did not
> 
> actually think i was going to pull it
> 
> off nice
> 
> that's awesome oh because it's kind of
> 
> similar same energy as uh
> 
> stick stream where he was the same thing
> 
> he was like working on just getting the
> 
> engine to compile
> 
> oh i forgot he did that
> 
> and then like last second of the stream
> 
> he said like it could pose
> 
> you could pass the joy on my face i wish
> 
> my camera was working
> 
> so so now people are like wait what did
> 
> you change yeah
> 
> yeah anyone tuning in now it's just like
> 
> okay
> 
> yeah so what are you actually working on
> 
> you don't know what i went through
> 
> okay it says yeah so dylan dylan's been
> 
> working on we're doing an engine
> 
> operator right now um to
> 
> we're going for the latest version of
> 
> unreal engine and every time we upgrade
> 
> the engine
> 
> basically it breaks a lot of stuff that
> 
> already worked
> 
> yeah and it's specifically a break stuff
> 
> that we've done
> 
> alterations to the engine so one in like
> 
> one
> 
> instance of that is our instance mesh
> 
> which is used for
> 
> pipes and conveyor belts ignore that
> 
> weird shadow thing
> 
> let's see that's going to go in the list
> 
> so that's yeah um and it's doing that
> 
> janky it was all gray there because it's
> 
> still compiling shaders if anyone's
> 
> curious it's not actually broken
> 
> um it will stop happening here
> 
> momentarily
> 
> once the display worker is done yeah
> 
> there's still
> 
> one billion shaders left and uh
> 
> the shader compile lists which i don't
> 
> think you can see on stream but
> 
> uh that one does not tell you the truth
> 
> because it's based on nested
> 
> shaders as well so like once it's like
> 
> i'm compiling one thousand shaders and
> 
> then once it's down to zero it's like
> 
> oh wait there's a dependency here and
> 
> then there's one thousand more shaders
> 
> yeah we're essentially working to get
> 
> back to the state of yeah
> 
> so if anyone tuning in now wants to know
> 
> what's the conveyor belts used to look
> 
> like
> 
> it was that and they were actually there
> 
> so if you tuned in now
> 
> you missed some really really really
> 
> riveting stuff
> 
> of me i'm like now i don't even care if
> 
> it wasn't an entertaining stream i'm
> 
> just so happy this works
> 
> no i'm sorry i hope it was entertaining
> 
> for people
> 
> so yeah it was okay it wasn't the best
> 
> you know working on
> 
> whatever i'm working on yeah you still
> 
> won't tell us that trailer you're
> 
> working on
> 
> hell yeah
> 