---
title: "November 27th, 2020 Video Jace Talk: UProperty refactored to be FProperty"
date: "2020-11-27"
layout: transcript
topics:
    - "technology/unreal-engine"
    - "technology/unreal-engine/object-limit"
---
# [November 27th, 2020 Video](../2020-11-27.md)
## Jace Talk: UProperty refactored to be FProperty
https://youtube.com/embed/0kmDHBWf640?autoplay=1&start=296&end=365

### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> cool uh next thing is a a pretty technical one it's um for those of you who know unreal engine 4 will this will make some sense i guess but i'll also talk about the implications of what that means for everyone and that is you property has been refactored to f property what this means is that everything that was tagged as you properties before came with the overhead of being an object when maybe it didn't need to be so this essentially means that things that were your properties before will be smaller because it contains less information they won't necessarily be considered an object and they won't be counted to uh the object list meaning iterating over objects as the game plays or whatever and this also means if there's less objects that means the build limit that people have um run into which is the it's not a build limit but it's a an object limit the object limit doesn't change but the number of objects in the game will reduce meaning you can build more so essentially what this means is we will go through and do the refactor and that means you can build more objects and an overall performance improvement
