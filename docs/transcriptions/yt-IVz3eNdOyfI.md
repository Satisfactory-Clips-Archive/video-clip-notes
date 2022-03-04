---
title: "April 27th, 2021 Livestream Q&A: Do you know why the new lights don't go through glass?"
date: "2021-04-27"
layout: transcript
topics:
    - "features/buildables/lights"
    - "features/buildables/walls"
    - "technology/unreal-engine/distance-fields"
---
# [April 27th, 2021 Livestream](../2021-04-27.md)
## Q&A: Do you know why the new lights don't go through glass?
https://www.youtube.com/watch?v=IVz3eNdOyfI
This question was possibly duplicated with a more recent answer: [April 20th, 2021 Livestream Q&A: If I spam lights will my factory die?](./yt-qn4e8a4Up7g.md) [https://www.youtube.com/watch?v=qn4e8a4Up7g](https://www.youtube.com/watch?v=qn4e8a4Up7g)


### Topics
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)
* [Features > Buildables > Walls](../topics/features/buildables/walls.md)
* [Technology > Unreal Engine > Distance Fields](../topics/technology/unreal-engine/distance-fields.md)

### Transcript

> do you know why the the new lights don't go through gas through glass I do, it's because the the lights in the game, aren't like classical lights they're kind of like made they're kind of special, they're almost not lights if I want to dumb it down enough but I don't want to do that, like the lights in the game are implemented in a certain way so that they're performing because a really expensive issue is when you're like looking at lights and they have like clusters of lights within them then, then they can potentially be very expensive so we're using some techniques to like, get around that I'm hoping to be able to do a youtube video about this at some point how they work because it's kind of interesting, but but tldr they essentially use like, it's called like a distance field, where they kind of like- I always try to like dumb this down and- I've never been able to like have a solid enough explanation of this that's simple to grasp because it's but essentially they're like kind of caching how the shadows and all that data, and and like they use distance fields okay just look that up and if you're interested whatever, but we kind of like need to to on a case by case like add what's part of that calculation and right now lights, like glass aren't part of that, like calculation yet for distance field, so that's why but we're going to do that eventually five-year-olds knew it excited yeah that's why it's so hard- I still haven't I need to think more about that because- I need there's there's no like good way to like explain it without going in depth I guess but they're kind of like cheat lights is what I'm trying to get at they don't work in the same way the other light lights work in the game, that's that's why they are made in the way they are there's also limitations to the way there are that's why you currently can't like rotate the, the, wall flood lights or whatever, because the way they do calculations doesn't work with that currently, so I don't know if we're gonna solve that in the future and I know you can rotate them in like the the micromanage mod, I don't know if the light breaks or whatever when you do that or something something anyway don't get stuck on this for too long but hopefully we'll make a youtube video explaining how the lights work cause I think it's really interesting and I think some people even though it might be a little bit like over most people, heads like it even is like a little bit over you know some game developers hats because like if you're not if you don't know how they work then you don't know how they work right, so we might make a really technical video at some point explaining that, and other systems in the game this is something specifically that you guys are interested in knowing more about like technically, please let me know and and we'll consider making like a a tech demo or something for some of the solutions we made for the game
