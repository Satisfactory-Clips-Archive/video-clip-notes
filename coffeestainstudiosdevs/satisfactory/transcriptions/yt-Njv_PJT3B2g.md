---
title: "October 9th, 2020 Livestream Q&A: What is the limit?"
date: "2020-10-09"
layout: transcript
topics:
    - "features/buildables/storage-containers"
    - "features/transportation/trains"
    - "technology/graphics"
    - "technology/unreal-engine"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Q&A: What is the limit?
https://www.youtube.com/watch?v=Njv_PJT3B2g
<details>
<summary>This question may have been asked previously at least 9 other times, as recently as October 2020 and as early as August 2020.</summary>

* [October 6th, 2020 Livestream Q&A: What is the object limit and why is it that number?](./yt-VpCuu0aYFw0.md) https://www.youtube.com/watch?v=VpCuu0aYFw0
* [September 22nd, 2020 Livestream Q&A: What is the Object Count Limit, and how can we tell in our own game?](./yt-gMq-fPCqGWQ.md) https://www.youtube.com/watch?v=gMq-fPCqGWQ
* [September 1st, 2020 Livestream Q&A: Have you thought about implementing a progress bar for how close to the Build Limit we are?](./yt-RyE_hc4huhA.md) https://www.youtube.com/watch?v=RyE_hc4huhA
* August 18th, 2020 Livestream Build Limit (Part 1): https://clips.twitch.tv/SplendidAffluentVampireNotLikeThis
* August 18th, 2020 Livestream Build Limit (Part 2): https://clips.twitch.tv/UnusualExquisiteKuduDendiFace
* August 18th, 2020 Livestream Build Limit (Part 3): https://clips.twitch.tv/SullenColdbloodedDiscEagleEye
* August 18th, 2020 Livestream Build Limit (Part 4): https://clips.twitch.tv/BlitheEnergeticEelPRChase
* August 18th, 2020 Livestream Build Limit (Part 5): https://clips.twitch.tv/GiantGeniusGooseCclamChamp
* August 18th, 2020 Livestream Build Limit (Part 6): https://clips.twitch.tv/BoxySmallAsparagusSmoocherZ
</details>


### Topics
* [Features > Buildables > Storage Containers](../topics/features/buildables/storage-containers.md)
* [Features > Transportation > Trains](../topics/features/transportation/trains.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> what is the limit it's kind of hard to
>
> say what the limit is because
>
> uh a lot of people confuse the limit
>
> with like object limits like
>
> in-game object limits which is not what
>
> is it what
>
> that is it's tied into the data
>
> objects data objects which isn't like
>
> one constructor are more data objects
>
> than a foundation for instance
>
> yes and no that's it's the primitive
>
> stuff too
>
> so we're trying to so it's pretty much
>
> i mean it's technically possible to say
>
> exactly what the limit is
>
> but it it really depends how you build
>
> because i've loaded
>
> save files that have that are
>
> less complex than all than say false
>
> that have hit the limit so to speak
>
> uh and it's mostly things that we are
>
> need to optimize for
>
> um because there are cases sometimes
>
> where like we just didn't think of like
>
> oh this is using a lot of stuff
>
> yeah we i think with the train update we
>
> had one issue where there's
>
> it was a simple thing of uh particle
>
> systems weren't being destroyed
>
> yeah so every time it took a turn it was
>
> scraping and that was just a miss
>
> like and i think it was just in
>
> blueprint even so it wasn't even yeah so
>
> yeah you find those things out too late
>
> after people with like big saves
>
> have trains running everywhere and then
>
> you're like why are they hitting the
>
> limit they shouldn't be hitting the
>
> limit
>
> then you could even see it as like
>
> people were playing it the game would
>
> slow down oh
>
> the fps was like chugging you're like
>
> why is this happening yeah take like 20
>
> minutes then the game was at a
>
> standstill
>
> there's also cases where uh if you like
>
> looked at a lot of or if you open a lot
>
> of storage containers you would also hit
>
> that limit sooner
>
> stuff like that yeah
