---
title: "May 28th, 2021 Livestream Snutt & Ben Talk: Light Pooling"
date: "2021-05-28"
layout: transcript
topics:
    - "features/buildables"
    - "features/buildables/lights"
---
# [May 28th, 2021 Livestream](../2021-05-28.md)
## Snutt & Ben Talk: Light Pooling
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=691&end=784

### Topics
* [Features > Buildables](../topics/features/buildables.md)
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)

### Transcript

> for the lights we use a an implementation that's quite common in games called pooling so basically what it does it has a lot of information points of like okay here could be a light there could be a light there could be light and we have an additional background threat for that uh hence uh people might have seen some crashes there but the background threat basically looks where the player is and then gets all those points okay these are relevant so we have a beautiful debug view for that where we can see all those points so these lights have one on the top and one on the bottom and here you can maybe see this one is of class of a light so there's a spotlight being pulled right here from this buildable and that way if i change the amount of lights are allowed it counts we might put these in the description too because people can use these commands in the game too so if you put one light then it will try to find the most relevant light for the player gotcha and this explains where some people have noticed that like if they have a ton of lights and they're running around the factory sometimes they can see like turn off in the distance and that's because of the cooling system that's like telling the game that like there's too many lights going on right now okay not everyone can be on at the same time okay
