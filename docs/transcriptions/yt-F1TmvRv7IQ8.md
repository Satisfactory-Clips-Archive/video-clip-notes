---
title: "June 1st, 2021 Livestream Q&A: Can you explain the Object Limit ?"
date: "2021-06-01"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [June 1st, 2021 Livestream](../2021-06-01.md)
## Q&A: Can you explain the Object Limit ?
https://www.youtube.com/watch?v=F1TmvRv7IQ8
This question was possibly duplicated with a more recent answer: [July 6th, 2021 Livestream Q&A: What does the Object Limit refer to exactly?](./yt-cVhPGZZyMn8.md) [https://www.youtube.com/watch?v=cVhPGZZyMn8](https://www.youtube.com/watch?v=cVhPGZZyMn8)


### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> can you explain the object limit so the object limit is, it's related to unreal engine's garbage collection so it's just a thing that keeps track of all the objects and helps clean them up in memory and all that kind of stuff right, and what what an object is it's not like an item in game right an object is an unreal engine game object right and and this doesn't really make too much sense to a player but if you're a developer you know like so so there could be like you know an object could be a like I think a foundation could be an object but sometimes like one single building can be made up of multiple objects so like a constructor I think historically had like four or four four or seven or something like objects in one object right so like that's and so we've done things to help like optimize that but that's what the object limit is and so the the the max limit there is just how many of those unreal engine game objects can we keep track of at a time
