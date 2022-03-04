---
title: "August 17th, 2021 Livestream Q&A: How do factories keep running if they're not actually loaded?"
date: "2021-08-17"
layout: transcript
topics:
    - ""
---
# [August 17th, 2021 Livestream](../2021-08-17.md)
## Q&A: How do factories keep running if they're not actually loaded?
https://www.youtube.com/watch?v=jcWCvjYzlvw
<details>
<summary>This question may have been asked previously at least 2 other times, as recently as February 2019 and as early as August 2018.</summary>

* [February 20th, 2019 Livestream Q&A: Will the machinery still work if I'm not loading that particular tile?](./yt-CB9bSigNYH8,2465.233333333333,2488.648026.md) [https://youtube.com/embed/CB9bSigNYH8?autoplay=1&start=2465&end=2489](https://youtube.com/embed/CB9bSigNYH8?autoplay=1&start=2465&end=2489)
* [August 1st, 2018 Q&A: Won't the factory stop working if you're really far away?](./yt-iFAy1NZUOGU,170.36,188.8.md) [https://youtube.com/embed/iFAy1NZUOGU?autoplay=1&start=170&end=189](https://youtube.com/embed/iFAy1NZUOGU?autoplay=1&start=170&end=189)
</details>


### Topics


### Transcript

> from dev to dev how do the calculations work so that all factories keep running if they're not actively loaded are you calculating every item constantly no it's like the the factories have their own tick like thread, if I'm not incorrect, yeah they have their own like factory thread that runs at its own speed and stuff so that kind of stuff isn't they're they're not like tied to the map that's loaded so all the stuff that's being built is like built on a different level to the rest of the map yeah like all the logic of all the factory buildings are always running I mean, yeah at the same time and that's how the calculations are done and then sometimes you see their visual representation when you walk closer yep you can check off another mansplaining there actually I think you explained it that more correctly than I did because- I said that that they're actually on a different level but they're not on a different level it's just a different different thread yeah I mean yeah they are like that they are okay I mean they are on a different they're on the like the the the the persistent levels I mean it's that's that is true
