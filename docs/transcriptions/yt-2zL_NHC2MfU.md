---
title: "November 9th, 2021 Livestream Q&A: Try using Unreal async save?"
date: "2021-11-09"
layout: transcript
topics:
    - "features/save-system"
    - "technology/unreal-engine"
---
# [November 9th, 2021 Livestream](../2021-11-09.md)
## Q&A: Try using Unreal async save?
https://www.youtube.com/watch?v=2zL_NHC2MfU

### Topics
* [Features > Save System](../topics/features/save-system.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> try using unreal engine async save not to so we've made our own custom save system and, the big problem with async saving is that there are it it works fine when you don't have any like dependencies on objects in your scene but when you have many dependencies as in like you know this factory building requires this input and this input requires this thing and it goes on and on and on, it makes it impossible to have async saving because you need to freeze what's going on to be sure that you capture the entire snapshot of objects in the serialization moment it's just too complex for satisfactory to do async saving in that way one solution we could do is to like when you're saving it like pauses all the machines or something like that, but that adds another like problem because that means that like we have to account for the different states of saving as well so it's just way easier just to just define that like during the save state we just freeze the game thread unfortunately which results in that like lame freeze that happens
