---
title: "May 28th, 2021 Dev Vlog Snutt & Ben Talk: New Holograms"
date: "2021-05-28"
layout: transcript
topics:
    - "features/buildables/foundations"
    - "satisfactory-updates/released/satisfactory-update-4"
    - "technology/graphics"
    - "technology/user-interface/holograms"
---
# [May 28th, 2021 Dev Vlog](../2021-05-28.md)
## Snutt & Ben Talk: New Holograms
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=945&end=1066

### Topics
* [Features > Buildables > Foundations](../topics/features/buildables/foundations.md)
* [Satisfactory Updates > Released > Satisfactory Update 4](../topics/satisfactory-updates/released/satisfactory-update-4.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > User Interface > Holograms](../topics/technology/user-interface/holograms.md)

### Transcript

> hence we are going now to the holograms so the main reason why we changed holograms that was because it was just causing a lot of memory issues um it became more apparent with update ford for some reason some things changed in the renderer that made it even worse also the conveyor belt items were an offender in that but if we get later to that so instead of swapping the instance mesh as they are now now they are instance of the conveyor all the constructors are one instance now what we used to do we used to uninstance the mesh and then make it a hologram which means every object of us instance is modified too for constructors that might not be the worst but for walls or foundations imagine you have twenty thousand foundations it means all those twenty thousand foundations are modified because you wanna hover on one foundation um so some people on really big saves just had lag spikes modifying their infrastructure right which is not fun so that was one of the main reasons the loading part is for every object that had to be instanced it had to create its render state so telling the render threat and the gpu that they should exist ironically the frame after it they were removed from the gpu so it adds tons and tons of data and i've removed it the frame after it so the loading time got increased with like 30 to 40 percent so it just did a ton of like unnecessary work at the first frame of the game and then just threw that kind of away yeah and that was also a reason for the dx12 in instability um right so that should be improved with that too i hope maybe tm futures
