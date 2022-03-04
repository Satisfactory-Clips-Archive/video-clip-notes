---
title: "May 28th, 2021 Dev Vlog Q&A: Are we going to be able to turn Lights upside down?"
date: "2021-05-28"
layout: transcript
topics:
    - "coffee-stainers/ben"
    - "features/buildables/lights"
---
# [May 28th, 2021 Dev Vlog](../2021-05-28.md)
## Q&A: Are we going to be able to turn Lights upside down?
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=500&end=598
This question was possibly duplicated with a more recent answer: [February 22nd, 2022 Livestream Q&A: Angle Lights up?](./yt-Bh6ulAtlCKE.md) [https://www.youtube.com/watch?v=Bh6ulAtlCKE](https://www.youtube.com/watch?v=Bh6ulAtlCKE)


### Topics
* [Coffee Stainers > Ben](../topics/coffee-stainers/ben.md)
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)

### Transcript

> static so one question that i've been getting, is regarding if we are going to implement so you can turn like lights upside down and stuff like that, because i believe there's a reason why that isn't working right now or something like that the reason is because i forgot to implement something that's the fairy that's the fair reason, so basically how our lights work they trace down so they get the right length, because the way how i want how i envisioned lights to work is they would be content context aware so they wouldn't just try to go all the way through the world because that would cause a lot of draw calls right because of the shadows so the lights do a line trace with a maximum distance, they should take the maximum distance if they fail to find anything, there are some cases where they don't and that's something i still have to patch up right so that's something that same might come in the future then yeah okay and same with the glass, currently they block less because it's a foundation piece but it should of course ignore glass but that's totally a future for now is that tricky because the you you'd need to like separate out the glass portion of the foundation portion and what not on those pieces or oh i i would just oh if it's a glass just trace through it right okay who cares let's trace through it nobody will know awesome is there anything else that you're planning to do with lights in the
