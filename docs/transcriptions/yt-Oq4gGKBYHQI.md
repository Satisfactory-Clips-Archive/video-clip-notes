---
title: "October 6th, 2020 Livestream Q&A: Map Editor?"
date: "2020-10-06"
layout: transcript
topics:
    - "environment/world-map"
---
# [October 6th, 2020 Livestream](../2020-10-06.md)
## Q&A: Map Editor?
https://www.youtube.com/watch?v=Oq4gGKBYHQI
This question was possibly duplicated with a more recent answer: [August 23rd, 2022 Livestream Q&A: Would it be possible to create our own Maps?](./yt-2BRnRTwf2UA.md) [https://www.youtube.com/watch?v=2BRnRTwf2UA](https://www.youtube.com/watch?v=2BRnRTwf2UA)


### Topics
* [Environment > World Map](../topics/environment/world-map.md)

### Transcript

> I saw someone before was asking about like map editor and stuff like that, that's a mild heart attack, every time we hear it but no not really no if that happens it's going to be like the mega distant future I don't think anyone should really think about it like obviously think about it because it's kind of cool right but, holy yeah but like that's not a I don't think anyone is going to even remotely think of that right now there's so many more important things yeah it's partly because the lavish level streaming we're using is so complex so it's really hard to like kind of use that system in a good way we we hardly do it in a good way, we made some I checked that part of the code yesterday we've done some weird hacks with the level streaming stuff, for some reason it's mostly for multiplayer because like you're not supposed to, unreal engine doesn't really have out-of-the-box support for listen server streaming which is what we're doing where like the way it works is like client and server they'll stream the level depending on where they are but the server also needs to stream the part where the client is at because they need to be able to do stuff and the server needs to authenticate that stuff so the server needs to stream both every client's world where they are right now but also itself, which is kind of weird because usually you have a dedicated server that just loads everything all the time and then yeah it keeps track of all that but we do it on a need to need basis and, yeah it's pretty pretty a lot of work went into that it's a lot of work dave a lot of work dave
