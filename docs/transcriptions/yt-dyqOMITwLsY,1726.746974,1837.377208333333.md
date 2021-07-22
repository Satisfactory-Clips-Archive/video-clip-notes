---
title: "May 28th, 2021 Livestream Q&A: How does picking items off the belt work?"
date: "2021-05-28"
layout: transcript
topics:
    - "environment/resources"
    - "features/buildables/conveyor-belts"
---
# [May 28th, 2021 Livestream](../2021-05-28.md)
## Q&A: How does picking items off the belt work?
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=1726&end=1838

### Topics
* [Environment > Resources](../topics/environment/resources.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)

### Transcript

> face in the game i remember there being a period where you hadn't implemented being able to pick up items on the belts is there anything interesting to share about that because it's you're not actually like since these aren't actually like physical objects in the world uh like how does that work when you're wanting to pick up this particular instance um we have handle states for that state handles i guess they're called um basically the old implementation was relying on the instance component that was under relying in a way just to check if it existed or not but that's it it didn't even use it so the only fix for that was just saying like okay you can always do it okay but otherwise how it works it all the belts are on splines let's see you see the white thin line oh i wish i had more vertices more words please so basically that line represents the belt so this is zero and that is one and we can calculate from where the player is looking which item to highlight right this is getting too much slower
>
> [Music]
>
> so we just make an approximation from looking at the belt because if you hover on the item you're not getting the item either so it's it's really based on the belt itself yeah um instead and i guess we cannot make thousands of hitboxes for that all the time yeah just not doable and i guess that's the limitation of doing it this way it's just that it's not like i said it's not an actual object in the world it's part of the belt so to speak yeah it's abstract data being represented yeah cool
