---
title: "November 27th, 2020 Video Jace Talk: Packet Reordering"
date: "2020-11-27"
layout: transcript
topics:
    - "features/multiplayer"
    - "technology/unreal-engine"
---
# [November 27th, 2020 Video](../2020-11-27.md)
## Jace Talk: Packet Reordering
https://youtube.com/embed/0kmDHBWf640?autoplay=1&start=217&end=270

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> thing that i want to talk about is packet reordering so that's been added to the engine now and what does it mean well by packet they're referring to network packages um so you guys have probably heard of thing called packet loss which is when your little packets of data gets sent to your friend and they don't make it um or they're discarded for one reason or another so packet reordering what that helps do is reduce the amount of packets that are lost so if um and in this case it's uh if multiple packets arrive out of order within the same frame they can now reorder the packets so that it makes sense so they don't have to discard it whereas typically when when packets arrive out of order the engine won't know what to do with those packets so it discards it and just like says can you send it again please yeah so this is going to help a lot with multiplayer performance essentially
