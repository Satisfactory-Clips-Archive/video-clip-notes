---
title: "January 10th, 2023 Livestream Q&A: Any idea how high of a priority it is to fix the smoothness of driving on Foundations?"
date: "2023-01-10"
layout: transcript
topics:
    - "features/buildables/foundations"
    - "features/requested-features"
    - "features/transportation/vehicles"
    - "technology/physics"
---
# [January 10th, 2023 Livestream](../2023-01-10.md)
## Q&A: Any idea how high of a priority it is to fix the smoothness of driving on Foundations?
https://www.youtube.com/watch?v=4qgk0863g0Y
<details>
<summary>This question may have been asked previously at least 2 other times, as recently as December 2022 and as early as July 2022.</summary>

* [December 20th, 2022 Livestream Q&A: Any update to bouncy tire bug on Foundations?](./yt--EYhEmqds18.md) [https://www.youtube.com/watch?v=-EYhEmqds18](https://www.youtube.com/watch?v=-EYhEmqds18)
* [July 12th, 2022 Livestream Q&A: Any plans to fix how Vehicles are done when driving on any Foundation surface?](./yt-vQjRcLqrXUM.md) [https://www.youtube.com/watch?v=vQjRcLqrXUM](https://www.youtube.com/watch?v=vQjRcLqrXUM)
</details>


### Topics
* [Features > Buildables > Foundations](../topics/features/buildables/foundations.md)
* [Features > Requested Features](../topics/features/requested-features.md)
* [Features > Transportation > Vehicles](../topics/features/transportation/vehicles.md)
* [Technology > Physics](../topics/technology/physics.md)

### Transcript

> any idea, how high of a priority it is to fix the smoothness of driving on foundations so we've talked about vehicle updates, before there will probably be no updates to Vehicles until we we intend to do like an overhaul of the vehicles and we're probably not going to be putting any time into fixing anything until we do that because in order to do that overhaul we're going to be undoing the work we would do in the meantime, and you know there's an argument to be said that we should do that first so that it's better in the meantime but we'll see, the the thing is my so the my understanding of that particular issue was something that I ran into when I was working on them way way back when, and what it is is that like there's when your wheels are driving there's a ray that gets cast down to find the ground to see where it is on the ground and now sometimes they're between foundations there's actually a tiny tiny Gap now the Gap is imperceptible but the ray is a one-dimensional ray it has no width that only has a length and so we can slide in between those gaps and so when it does that it says that the wheels are you know in it no longer on the ground in a weird different state and so that can cause the wheels to do something strange, so so my understanding is that that issue comes about, when driving on foundations because of that Ray doing funky stuff between foundations that's my understanding of it now there's a fix for that which is to not use a single Ray but instead to use a sweep of a shape so that it actually has a width, and a depth so that like it can't fit between those gaps the problem with that is that it is not very performant, so it was that was that that was in there but that was removed, in an effort to, in an effort to optimize the game so I don't know I don't know if we can just put that back in or if, you know when we do overhaul things we can make things better so
