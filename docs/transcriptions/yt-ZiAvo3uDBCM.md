---
title: "May 4th, 2021 Livestream Q&A: The flow rate issue in Pipes, is intended or will it be fixed?"
date: "2021-05-04"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "features/fluids"
    - "features/fluids/pipes"
    - "technology/graphics"
---
# [May 4th, 2021 Livestream](../2021-05-04.md)
## Q&A: The flow rate issue in Pipes, is intended or will it be fixed?
https://www.youtube.com/watch?v=ZiAvo3uDBCM

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Fluids](../topics/features/fluids.md)
* [Features > Fluids > Pipes](../topics/features/fluids/pipes.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> the fluorine pipe sucks mostly when you build it for max loader it is intended it will be fixed it will be fixed at some point I think it's a very tricky issue, because it's an underlying problem with, the system the same problem kind of exists on conveyor belts as well because if you don't have like a good, frame rate then you can run into precision issues with the calculations where it doesn't have I don't know exactly what the problem is but it's tied to like the the rounding of numbers and the precision of floats floating point numbers that we use for calculation of like fluids and and items on conveyor belts so sometimes if you've like put 100 efficiency on a certain production line and you run into cases where it doesn't produce 100 efficiency it's usually tied to that and it's tied to like you know your frame rate has a significant impact on this as well as like some of the some major like drawbacks of those implementations that we've made and it's like we've had to take some of those, decisions based on the systems themselves as well so it's not like what I'm trying to say is it's not an easy fix and, it's not a it's not a fix that we know for sure that we're to be able to do but it's something that we definitely want to fix at some point
