---
title: "November 10th, 2020 Livestream Q&A: Is it true that building vertically equals worse performance than building horizontally?"
date: "2020-11-10"
layout: transcript
topics:
    - "features/unplanned-features/mass-building"
    - "technology/graphics"
---
# [November 10th, 2020 Livestream](../2020-11-10.md)
## Q&A: Is it true that building vertically equals worse performance than building horizontally?
https://www.youtube.com/watch?v=BF0MYqw_SpM

### Topics
* [Features > Unplanned Features > Mass Building](../topics/features/unplanned-features/mass-building.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> um someone was asking oh here is it true that building vertically equals worse performance as opposed to building horizontally and spread out i don't uh yes to some degree um because the way um if you were to like if you were to take say that you built all spread out throughout the map uh and you build a lot and then you take all that and just chunk it into one vertical tower or whatever that will definitely more expensive because uh the way we kind of optimize the game is to not do stuff that's like the best way to offer the best way to optimize the game is to remove stuff right how to optimize life yeah exactly so what we're doing is essentially like when you're not seeing you know constructors we don't render them when you're not seeing trains move around then it's just like they're not actually calculating you know like physics and whatever not the change to that i mean the other vehicles um so like the less you see the the better um essentially um and there are also there are systems to like calculate like when you're looking at something to check like like oh what is obstructing including and stuff to not render but uh there you hit a limit at some point where like there's so many objects that has to go through and check so it becomes less performant than when you actually occlude them so in some cases it's actually worse to turn that off and in some cases if people build really big bases you have to turn that off because it crashes the game otherwise as seen in the fluids experimental fluids video that was really good yeah so i think it also depends a little bit like if uh like for instance i've done like a five by five challenge thing where i built everything in the tower i don't really see any performance difference at all but i also don't have an insane amount of stuff in my factory even though i'm building vertically so it depends a little bit but if you have like a mega factory you know think kibbits style then for sure building vertically is less performances cubits i'm spraying it i don't know some some person that people p people keep saying uh exists hmm yes are you guys what do i just get a [ __ ] goof you're just gonna goof yeah this is serious business there's no time to goof sorry i'm a professional
