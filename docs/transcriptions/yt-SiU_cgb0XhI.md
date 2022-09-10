---
title: "May 18th, 2021 Livestream Q&A: Is there a technical reason you only made Mk.5 belts and not higher?"
date: "2021-05-18"
layout: transcript
topics:
    - "coffee-stainers"
    - "features/buildables/conveyor-belts"
    - "features/buildables/storage-containers"
    - "features/buildings/miner"
    - "features/crafting/recipes"
---
# [May 18th, 2021 Livestream](../2021-05-18.md)
## Q&A: Is there a technical reason you only made Mk.5 belts and not higher?
https://www.youtube.com/watch?v=SiU_cgb0XhI
This question was possibly duplicated with a more recent answer: [September 6th, 2022 Livestream Q&A: Mk.6 Conveyor Belts?](./yt-5kppmSyt6_E.md) [https://www.youtube.com/watch?v=5kppmSyt6_E](https://www.youtube.com/watch?v=5kppmSyt6_E)


### Topics
* [Coffee Stainers](../topics/coffee-stainers.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Buildables > Storage Containers](../topics/features/buildables/storage-containers.md)
* [Features > Buildings > Miner](../topics/features/buildings/miner.md)
* [Features > Crafting > Recipes](../topics/features/crafting/recipes.md)

### Transcript

> is there technical reason because you only made mk5 belts and no higher, there is a technical reason for, why they don't go higher but there also might be a design reason for it not to be first to not be mk6 but there is there is definitely also a technical reason which you know may or may not be solvable but it becomes really hard to sort of, at a certain point to calculate how many units can travel along the belt pass through, merges and splitters and stuff like that, it actually actually becomes a very tricky problem like I remember quite a few years ago when the programmer at the time who was working on those belts he was obsessed with splitters and mergers for like a couple weeks straight and it was it was and I'm you know I was like you know what's what's the problem he would talk to me about it and it was actually really complicated yeah it usually is like you don't really think about when you just see like the result or like the black box or something you don't really realize like how much work goes in every because every that's the same thing every time I recently actually talked to, one of the programmers that have been working on splitters a little bit recently and I was like hey why can't we just do this thing and he was like well you got a moment you want to sit down and they told me like all like the weird edge cases that can happen and like why why it's it's it is the way it is, so yeah it's it's complicated you guys, but also to follow up like a question I got a lot too is is the mark iii minor with like how you can't get currently in the game you can't get the full output from them if you overclock them and that's something that we're gonna, touch upon later down the line we don't know for sure if like jace mentioned if like we're gonna solve the technical issue that's that's the reason why we can't do that currently or if we're gonna like have to rebalance all the belts in the game to match like what the highest speed we currently have you know, and then make that the the maximum and that's kind of what we did with pipes for a while too where we know for we know for a fact we won't be able to go over 600 cubic meters per per minute we we are already kind of like does it actually work fully like I don't know it's a bit like we're kind of testing it still, and at some point maybe we'll change that and just make it so that you know 600 is yeah still the maximum but there might be like some lower value to it that some machines use or something like that so there might be some rebalance there, but in those three balances I'm pretty sure that it won't really affect every anyone that much it will just make like all your things offset a little bit in your recipes and then, like if it worked before it will still work in those cases it's not like the rebalancing of recipe stuff, is my understanding of it when they explain it to me but totally explicit with the big brain here yeah let me just add a second output bam bam bam well bam so actually they've told me no that's not an easy solution either apparently oh really because of race conditions that can happen with the belts so there's it's already an issue with the com like the storage containers that can have one and two outputs it's already a problem there so that's why they don't want to do that either nice yet at least maybe they solve it
