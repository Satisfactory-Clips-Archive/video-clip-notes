---
title: "October 9th, 2020 Livestream Q&A: What is the limit?"
date: "2020-10-09"
layout: transcript
topics:
    - "features/buildables/storage-containers"
    - "features/transportation/trains"
    - "technology/graphics"
    - "technology/unreal-engine/object-limit"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Q&A: What is the limit?
https://www.youtube.com/watch?v=Njv_PJT3B2g
This question was possibly duplicated with a more recent answer: [July 6th, 2021 Livestream Q&A: What does the Object Limit refer to exactly?](./yt-cVhPGZZyMn8.md) [https://www.youtube.com/watch?v=cVhPGZZyMn8](https://www.youtube.com/watch?v=cVhPGZZyMn8)


### Topics
* [Features > Buildables > Storage Containers](../topics/features/buildables/storage-containers.md)
* [Features > Transportation > Trains](../topics/features/transportation/trains.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> what is the limit it's kind of hard to say what the limit is because, a lot of people confuse the limit with like object limits like in-game object limits which is not what is it what that is it's tied into the data objects data objects which isn't like one constructor are more data objects than a foundation for instance yes and no that's it's the primitive stuff too so we're trying to so it's pretty much I mean it's technically possible to say exactly what the limit is but it it really depends how you build because I've loaded save files that have that are less complex than all than say false that have hit the limit so to speak, and it's mostly things that we are need to optimize for, because there are cases sometimes where like we just didn't think of like oh this is using a lot of stuff yeah we I think with the train update we had one issue where there's it was a simple thing of, particle systems weren't being destroyed yeah so every time it took a turn it was scraping and that was just a miss like and I think it was just in blueprint even so it wasn't even yeah so yeah you find those things out too late after people with like big saves have trains running everywhere and then you're like why are they hitting the limit they shouldn't be hitting the limit then you could even see it as like people were playing it the game would slow down oh the fps was like chugging you're like why is this happening yeah take like 20 minutes then the game was at a standstill there's also cases where, if you like looked at a lot of or if you open a lot of storage containers you would also hit that limit sooner stuff like that yeah
