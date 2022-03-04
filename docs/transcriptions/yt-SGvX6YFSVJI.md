---
title: "June 29th, 2021 Livestream Q&A: What does LOD Dithering do in the game?"
date: "2021-06-29"
layout: transcript
topics:
    - "technology/graphics/lod"
---
# [June 29th, 2021 Livestream](../2021-06-29.md)
## Q&A: What does LOD Dithering do in the game?
https://www.youtube.com/watch?v=SGvX6YFSVJI

### Topics
* [Technology > Graphics > LOD](../topics/technology/graphics/lod.md)

### Transcript

> what does lod dithering do in the game it's, when, when objects are in the distance we load in like a lower, a model of the same thing that has less vertices like the amount of polygons on the object and when you're getting close to that there's a there's an effect that's called dithering where it will render both of them at the same time and then it will like only render parts of it right and the closer you get to it the more parts of the the thing that isn't like is it like the it's like the dots or yeah exactly, and it mostly happens on on foliage in our game yeah you'll have probably seen it before it's like when they sort of like blend in but it's like the the I'm pretty sure if I eric kirk if I'm wrong here but dithering refers to like like the dots kind of thing yeah they come in like kind of like always like these I can't explain it yeah it's a way to cheat transparency without actually having transparency because transparency is very expensive to render because you have to render both the object that's in front of it and the objects that's behind it to know like how transparent the the thing is whereas with dithering you just render once and but you don't render the whole thing and there's various like the other techniques where how the dots are like how how you pick which part of the object to render at certain points laud loading of thoughts loading of dots how many dots can it
