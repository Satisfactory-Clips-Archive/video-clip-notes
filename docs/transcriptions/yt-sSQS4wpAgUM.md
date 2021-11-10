---
title: "October 12th, 2021 Livestream Q&A: If one Train enters 5 seconds before, will trains stop before Signal?"
date: "2021-10-12"
layout: transcript
topics:
    - "features/transportation/trains"
    - "features/transportation/trains/train-signals"
    - "satisfactory-updates/released/satisfactory-update-5"
    - "satisfactory-updates/teasers-and-trailers/update-5-teasers"
---
# [October 12th, 2021 Livestream](../2021-10-12.md)
## Q&A: If one Train enters 5 seconds before, will trains stop before Signal?
https://www.youtube.com/watch?v=sSQS4wpAgUM

### Topics
* [Features > Transportation > Trains](../topics/features/transportation/trains.md)
* [Features > Transportation > Trains > Train Signals](../topics/features/transportation/trains/train-signals.md)
* [Satisfactory Updates > Released > Satisfactory Update 5](../topics/satisfactory-updates/released/satisfactory-update-5.md)
* [Satisfactory Updates > Teasers & Trailers > Update 5 Teasers](../topics/satisfactory-updates/teasers-and-trailers/update-5-teasers.md)

### Transcript

> hell yeah but if one enters like five seconds before will other trains stop it probably before the signal no so like before the train gets there it's going to have reserved that block it for itself it's not like the second it's not like the second the train goes over the line that's when it gets initialized like the trains decide when they're whether or not they're taking they're going to go through a block a little bit before and uh yeah then the other ones will slow down and stuff yeah i think it's easy game yeah it's using the game loop to do that check and the game loop is sequential so uh yeah you can't have like i guess you could potentially have a deadlock at some point but yeah shouldn't trans predict where other trains are going to be two trends are approaching simple okay it's the same question over and over so like guys like the the system as far as i i see it works right so like you don't get two trains going into the same block somehow i don't know how that works but like as far as i understand feel free to try and do it but as far as i can see and i've never heard of anyone getting two trains to go into the same block without manually piloting one of them or something like that
