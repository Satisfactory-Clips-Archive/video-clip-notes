---
title: "May 6th, 2022 Livestream Q&A: Doesn't Unreal Engine have a limit & Mk.5 belts are already approaching that?"
date: "2022-05-06"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/unreal-engine"
---
# [May 6th, 2022 Livestream](../2022-05-06.md)
## Q&A: Doesn't Unreal Engine have a limit & Mk.5 belts are already approaching that?
https://www.youtube.com/watch?v=cpWRCbSYMsE

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> doesn't a real engine have a limit and mark five is already approaching that there is a there is a limit yes but it's not unreal engine tied it's tied to like how
>
> [Music]
>
> it's it's tied to like more per like it's tied to the fact that we're using floating point, numbers for the inputs and outputs of conveyor belts and that causes some like visual issues and I mean that issue that's the main reason why we haven't added mark 6 belts because we haven't been able to solve that issue but it's possible that we can solve that issue, it's possible it so it's possible that we might be able to solve that issue it's possible that we might not be able to solve that issue and you know based on that that can also you know affect our decision whether we'll go with mark six belts or not so we don't know like we haven't that's that's the main reason why you also haven't given an answer on this is because we haven't actually delved into that problem programming problem yet and you know that's a big deciding factor on whether we can do it or not so there's some dependency there
>
> [Music]
>
> so we'll see we'll see make mark 6 build that actual item rendering of rendering is the issue, possibly yes it might also be that it's not the rendering that's actually the issue might also be the case where because we have tried having belts without rendering and it is it is it is very unclear what's going on when you don't have items moving and you can't see that something is happening, it creates like this weird like like you not yeah you don't see what's going on essentially, and that can be also more performant but it's like bad ux user experience yeah disparity exactly, so I don't know if we we I don't think we like that solution honestly marxist such as teleporter so I hate to break it to you guys but even if there was just like teleporters the only thing you're saving is the rendering of the items moving apart from that they would function the same way essentially you're still doing input output calculation stuff like how items are moving in speed and like you can still run into those precision issues especially when you don't have, good performance like if you're in low fps so that would actually not solve the problem it would just it would reduce the amount of items rendered which could potentially improve it but factory like tick-wise it would still be the same you
