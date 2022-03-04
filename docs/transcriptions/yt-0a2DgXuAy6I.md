---
title: "July 6th, 2021 Livestream Q&A: How do Belts affect performance?"
date: "2021-07-06"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/graphics"
---
# [July 6th, 2021 Livestream](../2021-07-06.md)
## Q&A: How do Belts affect performance?
https://www.youtube.com/watch?v=0a2DgXuAy6I

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> how do belts affect performance note I've heard if you have lower fps you have precision issues with higher tier belts but do high tier belts affect fps more drastically I don't think belt speed affects no the bell speed doesn't well rendering effects like the more belts you have obviously the the the more you have to render yeah and and that affects your your overall performance I guess and you know and that overall performance then affects belt precision, yeah but what was the question again like well does does high tier belts affect fps more they don't no like all belts are equal in the sense that like performance-wise yeah cause like the way the if you haven't checked out the video we put out on our youtube with ben like he explained a little bit how they work but maybe not delving in too deep into it but the way they work is they they kind of trick you because they're not actually objects moving on the belt it's just we render the belt and then we render the the items instantly like the the items are part of the belt sort of when we render them with with a little bit of rendering tricks so like it's not a case of like the more items on the belts the more you have to render sort of, if that makes sense, yeah it's you're still just rendering a belt yeah whether regardless of how the belt looks the items on the belt are part of it kind of yeah it's it's rather the like the the lot like the size of the belt and like how many you have and when we update them etc etc that like affects rendering because then it's like since not all belts are instanced in one like if you have a long belt line like the it will still be like, rendered in in, segments right now we are planning to make it so that they are they instance the entire thing at some point, so like it really is like the amount of belts rather than like what belt you're building
