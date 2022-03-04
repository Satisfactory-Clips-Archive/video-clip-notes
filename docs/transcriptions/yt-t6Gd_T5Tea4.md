---
title: "October 9th, 2020 Livestream Dylan Talk: Buffer Overflow bugs"
date: "2020-10-09"
layout: transcript
topics:
    - "features/multiplayer"
    - "technology/unreal-engine"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Buffer Overflow bugs
https://www.youtube.com/watch?v=t6Gd_T5Tea4

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> yeah oh and for people to have the the buffer overflow just, don't dismantle things no that i was investigating a, the could not connect, client buffer overflow issue but the one save that i had that was getting it it was because they had a giant storage box filled with i don't even know how many there's a max array size for, replicating and it's pretty small i think it's, you went 16 so i think 65 000. it might even be smaller might be 32 000 so you can, it just couldn't actually send that array to the client so the client would automatically disconnect so, if you're the host though you can fix that by, emptying that box we're talking about local like the small storage yeah when you like mass dismantle a bunch of storages and it fills a small tiny little container somehow with everything that was there that is the cause i think of most instances of that we might have another reason but so we need to get a fix in for that as well yes sir oh you have done a fix it's just not up yet yep that's also coming there's a lot of like small fixes that are coming but it's really hard to
