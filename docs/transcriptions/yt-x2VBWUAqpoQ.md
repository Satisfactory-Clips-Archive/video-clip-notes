---
title: "August 24th, 2021 Livestream Q&A: Is there going to be a Mk.6 Belt for Mk.3 Miner at 250% clock speed?"
date: "2021-08-24"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "features/buildings/miner"
    - "features/buildings/overclocking-underclocking"
---
# [August 24th, 2021 Livestream](../2021-08-24.md)
## Q&A: Is there going to be a Mk.6 Belt for Mk.3 Miner at 250% clock speed?
https://www.youtube.com/watch?v=x2VBWUAqpoQ
<details>
<summary>This question may have been asked previously at least 13 other times, as recently as May 2021 and as early as September 2020.</summary>

* [May 18th, 2021 Livestream Q&A: Is there a technical reason you only made Mk.5 belts and not higher?](./yt-SiU_cgb0XhI.md) [https://www.youtube.com/watch?v=SiU_cgb0XhI](https://www.youtube.com/watch?v=SiU_cgb0XhI)
* [May 4th, 2021 Livestream Q&A: Mk.6 Conveyor Belts?](./yt-9KayDn0JaEY.md) [https://www.youtube.com/watch?v=9KayDn0JaEY](https://www.youtube.com/watch?v=9KayDn0JaEY)
* [April 27th, 2021 Livestream Q&A: Will there ever be a belt that goes faster, like a Mk.6 one?](./yt-cnyCqL7xl6U.md) [https://www.youtube.com/watch?v=cnyCqL7xl6U](https://www.youtube.com/watch?v=cnyCqL7xl6U)
* [April 6th, 2021 Livestream Q&A: Mk.6 Belts?](./yt-sUed4aFcYLs.md) [https://www.youtube.com/watch?v=sUed4aFcYLs](https://www.youtube.com/watch?v=sUed4aFcYLs)
* [March 30th, 2021 Livestream Q&A: Will there be a Mk.6 belt?](./yt-x2MeE6UR3o8.md) [https://www.youtube.com/watch?v=x2MeE6UR3o8](https://www.youtube.com/watch?v=x2MeE6UR3o8)
* [March 30th, 2021 Livestream Q&A: Will there be Belt Mk.6?](./yt--fmlo0D_LXM.md) [https://www.youtube.com/watch?v=-fmlo0D_LXM](https://www.youtube.com/watch?v=-fmlo0D_LXM)
* [March 23rd, 2021 Livestream Q&A: Any chance of faster belts in the future?](./yt-Rv5-4k_ZzWU.md) [https://www.youtube.com/watch?v=Rv5-4k_ZzWU](https://www.youtube.com/watch?v=Rv5-4k_ZzWU)
* [February 2nd, 2021 Livestream Q&A: Mk.6 Belt in the next Update?](./yt-DpT2LNED0wk.md) [https://www.youtube.com/watch?v=DpT2LNED0wk](https://www.youtube.com/watch?v=DpT2LNED0wk)
* [November 24th, 2020 Livestream Q&A: Mk.6 Belts coming?](./yt-H2WwaLFOI9Q.md) [https://www.youtube.com/watch?v=H2WwaLFOI9Q](https://www.youtube.com/watch?v=H2WwaLFOI9Q)
* [November 10th, 2020 Livestream Q&A: Are Conveyor Belt Mk. 6 going to be a thing?](./yt-WbtzFVFOFMs.md) [https://www.youtube.com/watch?v=WbtzFVFOFMs](https://www.youtube.com/watch?v=WbtzFVFOFMs)
* [November 3rd, 2020 Livestream Q&A: Any plans for better Belts for Pure nodes?](./yt-UxW9nGO9Ius.md) [https://www.youtube.com/watch?v=UxW9nGO9Ius](https://www.youtube.com/watch?v=UxW9nGO9Ius)
* [November 3rd, 2020 Livestream Q&A: Broader Belts?](./yt-Y1ulbhgaSeU.md) [https://www.youtube.com/watch?v=Y1ulbhgaSeU](https://www.youtube.com/watch?v=Y1ulbhgaSeU)
* [September 29th, 2020 Livestream Q&A: What about Mk.6 Belts?](./yt-NiBLAUCxIEs.md) [https://www.youtube.com/watch?v=NiBLAUCxIEs](https://www.youtube.com/watch?v=NiBLAUCxIEs)
</details>


### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Buildings > Miner](../topics/features/buildings/miner.md)
* [Features > Buildings > Overclocking & Underclocking](../topics/features/buildings/overclocking-underclocking.md)

### Transcript

> um is there going to be a mark six belt for minor mark three at two to five percent clock speed so um sorry i'm thinking about the tweet chase put out um i we don't know honestly like they're so here's the full story right behind why we haven't put that in the game yet um the way the conveyor belts work is that we like everything all the logic is running sort of behind the scenes and then we render on top of that right so like the conveyor belts are like not really like they're not really there but they are okay um so the way that we calculate like things on the conveyor belts right is is we you know to have it right work and like be able to render so many items at the same time in the world we sort of have to like figure out optimization techniques to get around it so one of the ways we use to to calculate like where items are in the belt is uh we we're using floating point numbers um and one of the issues with floating port numbers is that there is a precision issue um when you need to go higher like decimal values i'm not going to go into like how floating point values work if you want to know more about that i think there's a really good youtube video actually it's very like computer science related though so uh but just google on youtube and there's a bunch of like computer file did one um et cetera et cetera but but essentially like the way they work is that the more like decimal values you need the less precise the value will be of the number that you're using right because it's a limited amount of bits that you store the float import numbers in um and when you're making calculations on you know on imprecise values then you know that layer on top of each other and the problem we have specifically is that the faster the belts are going the higher the precision is needed to be able to get like good values of like where things are in the valuables right so we sort of hit the limit on the conveyor belts right now in the current implementation um and which makes it that we can't you we can't make like a faster belt the way the system works right now we'd have to rework a little bit how the how the how the system works um so what would have what we would have liked to do i believe is to have just you know mark six belt um so so that you can clock a minor up to 250 and then you'll get a full full um conveyor belt and if we can't do that then maybe so the solution would be to have two conveyor belts out of the miner um we don't know we haven't decided because we haven't we haven't invested in this problem yet we haven't invested time in this problem yet because we feel like you know this isn't as big of an issue as you know say i don't know ramp railings you know ramp range is much more important feature to work on so we felt like it's more important to work on that feature um and that's what we did so that's sort of what we need to prioritize on when we're working on but at some point we're gonna need to solve that problem when we lead up into 1.0 so you know we're going to solve that problem eventually at some point what the solution is going to be whether or not we're going to like nerf sort of speak the the conveyor belts or if you can add another output what the best solution is we don't know and you know we won't know until we start working on it so when we know then we'll tell you guys
