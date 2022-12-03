---
title: "September 22nd, 2020 Livestream Q&A: Would implementing covered belts reduce the number of objects in the world?"
date: "2020-09-22"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "features/unplanned-features/mass-building"
    - "technology/graphics"
    - "technology/unreal-engine/object-limit"
---
# [September 22nd, 2020 Livestream](../2020-09-22.md)
## Q&A: Would implementing covered belts reduce the number of objects in the world?
https://www.youtube.com/watch?v=2R4MfLt_oMw
This question was possibly duplicated with a more recent answer: [November 29th, 2022 Livestream Q&A: Would adding the ability to add a cover on Belts help performance?](./yt-1UhSGB8cxAk.md) [https://www.youtube.com/watch?v=1UhSGB8cxAk](https://www.youtube.com/watch?v=1UhSGB8cxAk)


### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Unplanned Features > Mass Building](../topics/features/unplanned-features/mass-building.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> let's keep it that way, we're implementing, covered belts reduce the amount of objects in the world no I don't think I don't if correct me if I'm wrong here's snit but I'm pretty sure the objects on a belt don't count to the object counter is that correct because I'm pretty sure they use the hierarchical instance something something yes but they still count as like an object because it's still calling them, but as like a you object because are they the things that get counted does it really yeah it's the garbage collector that's like the problem because the garbage collector has a limit of how many objects they can keep track of so to speak and that's the that's that limit, but I don't think I don't quite remember the implementation of the objects on the belts, because I think all those are instances and they only count as like they're all instances that's what I'm saying yeah yeah yeah yeah I don't remember I think that's why I think they're just there might be some some data values under like underneath the belt so to speak that's not like the rendered thing but what it's keeping track of maybe but I don't think yeah there there are there are like a a weird array thing yeah but the thing is so ben actually our technical artist has actually, tried out doing like, that exact thing like, covered belts to see what kind of improvement you get from that and I don't remember if if what the conclusion was but he has tried it out so I mean if it was it was beneficial then maybe we'll see it in the future and if it wasn't then I guess not but, we have gone down that route and tried it out
