---
title: "October 6th, 2020 Livestream Q&A: How does the AoE on the Chainsaw work?"
date: "2020-10-06"
layout: transcript
topics:
    - "features/equipment/chainsaw"
---
# [October 6th, 2020 Livestream](../2020-10-06.md)
## Q&A: How does the AoE on the Chainsaw work?
https://www.youtube.com/watch?v=GRvWhu6FKOk

### Topics
* [Features > Equipment > Chainsaw](../topics/features/equipment/chainsaw.md)

### Transcript

> how does the aoe on the chainsaw work well I'm glad you asked because I'm actually the one who implemented that, it's based on the play it's based on the position where you chainsaw on wait constructors do this god damn it wait what they make solid biofuel yeah you can do that infrastructure yeah I know I knew on you, it's it's like the point on the thing that you're chainsawing that's the center of the aoe and then it's it's a fixed size, sphere essentially just checks if there's stuff within there, it's a bit finicky because foliage has weird collision based on- I don't know what the collision and the foliage is based on I think it's a mesh or something so sometimes it will totally be inside that aoe circle and it didn't doesn't get chopped up and because of collision or whatever so that's how that works
