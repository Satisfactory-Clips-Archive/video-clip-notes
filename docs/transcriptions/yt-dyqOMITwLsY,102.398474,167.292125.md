---
title: "May 28th, 2021"
date: "2021-05-28"
layout: transcript
topics: 
    - "features/buildables/lights"
    - "satisfactory-updates/released/satisfactory-update-4"
    - "technology/unreal-engine/object-limit"
    - "technology/graphics"
---
# [May 28th, 2021 Dev Vlog: How Lights work in Satisfactory](../2021-05-28.md)
## Q&A: What was the main issue with implementing Lights?
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=102&end=168
### Topics
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)
* [Satisfactory Updates > Released > Satisfactory Update 4](../topics/satisfactory-updates/released/satisfactory-update-4.md)
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> so what was like the main issue with
> implementing lights and like why
> couldn't we just slap
> lights into the game with like the
> objects that we had sort of
> so first case is the
> the infamous object limit that's one of
> the reasons
> because if you want to build an object
> you need to have the object in the world
> and we couldn't allow that because that
> would just add thousands of thousands of
> objects that would
> do nothing most of the time so we had to
> find a nice solution for that
> and second of it lights are really
> expensive when they're overlapped with
> each other
> that's something that we had to find
> some kind of solution
> for too and also to make it nice for
> multiplayer
> like just imagine somebody has to spend
> a spawn point with 5000 lights on the
> hub
> the player that joins it that can't
> leave it because their computer will
> just blow up
> right so for all those things we had to
> implement the system to
> manage lights and in the end it was a
