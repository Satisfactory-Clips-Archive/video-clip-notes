---
title: "June 8th, 2021 Livestream Q&A: Please, teleporters?"
date: "2021-06-08"
layout: transcript
topics:
    - "features/requested-features"
    - "satisfactory-updates/satisfactory-prototypes"
---
# [June 8th, 2021 Livestream](../2021-06-08.md)
## Q&A: Please, teleporters?
https://www.youtube.com/watch?v=dNPT8HQ3qRk
This question was possibly duplicated with a more recent answer: June 28th, 2022 Livestream Q&A: Any plans for Teleporters? [https://www.youtube.com/watch?v=0orGp3fSLmE](https://www.youtube.com/watch?v=0orGp3fSLmE)


### Topics
* [Features > Requested Features](../topics/features/requested-features.md)
* [Satisfactory Updates > Satisfactory Prototypes](../topics/satisfactory-updates/satisfactory-prototypes.md)

### Transcript

> these teleporters I remember when we had teleporters back in the day like before the game was out and we were like we had prototype teleporters we didn't really have them in but the, designers just, prototype teleporters it helped me solve a crash bug in the vehicles I've told that story yeah I think I've told us I think you can tell it again because you have to tell it again it's been a while right yeah yeah so like we had these we had these teleporters and there was this test map that I would work on and, one day I made a change to vehicles lo and behold there was like a crowd they were causing a crash and we didn't know what the hell was going on, and, wait how did this work yeah so so, I was like okay so what's happening so simon showed me the simon who found it and if he parked, like an explorer on this one ramp on this level and like and then got out the explorer would just disappear and reappear somewhere else on the map but if you stayed in the explorer the game would crash and the crash logs would look at like what's crashing and it was like a berry it was crashing in a berry or something like that we're like what the hell is going on why is it berry crashing when the the vehicle disappears and, so what what ended up, solving it was like sometimes it would crash at this berry other times it would, it wouldn't crash but the vehicle would drive out of a teleporter and we're like why is this happening and you know why is it when I parked the vehicle it comes out of the teleporter and what happened was there was like a divide by zero error in the, in the vehicle and so in a very specific case which happened if you parked on this one ramp the physics in the vehicle would divide by zero and infinite forces would be applied to the to the vehicle and so the the hitbox of the vehicle expanded to infinity within a frame and occasionally that hitbox then overlapped with one of the teleporters which reset the physics in the vehicle positioned it to the other teleporter and then it would just drive out of the teleporter so that's kind of how that was happening and and that's how I figured that out so, I just have to go and fix that divide by zero and then everything was fine again but yeah thanks teleporter and then sometimes it would crash on the, the, the berry thing because like the hitbox would would collide with the berry first and then the physics object would like die or some [ __ ] and yeah it was really weird it was a really weird thing so, yeah I had, thanks teleporter what what a nice way to like fail graciously just having it be like yeah I was like why does it drive out of the the teleporters it's so weird oh it's so funny though yeah
