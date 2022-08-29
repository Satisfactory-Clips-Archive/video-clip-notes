---
title: "November 10th, 2020 Livestream Jace Talk: Encased Conveyor Belts"
date: "2020-11-10"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/graphics"
---
# [November 10th, 2020 Livestream](../2020-11-10.md)
## Jace Talk: Encased Conveyor Belts
https://www.youtube.com/watch?v=xT-2uWvm3iw

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> so I got some folks asking about like encased conveyor belts or conveyor tubes, we've talked about that before as well I think, I always forget what it is that you're the one who talks about it normally it is it's you dude right no comment I don't wanna no yeah, we've tried that, I don't know the exact like I keep forgetting to ask ben about it because he's tried it, he's done some like tests with it ben if you're listening give us a sign give us a sign give us a sign yeah get the speaker ball I got the speaker box over here let me just put it down, emf5 ben must be nearby
>
> [Laughter]
>
>, we have tried it but I don't know if we like we saw like a big performance improvement and felt like it's worth pursuing it, or maybe we did and we just haven't had like because that's the thing like even if there's a lot of good stuff we want to do we just don't have time to do it, because we have to do other stuff, so I don't know the state of that actually but it feels like if there was a huge significant improvement with that I think we would have pursued it yeah yeah because there is like there's like a lot of stuff that's put in place into, making drawing each individual item, on the belts to be very efficient there is, so it's like my understanding is that it's it's not as heavy as you would think that because because the oil is always the same thing or yeah yeah there's a lot of assumptions you can make and so that becomes a very efficient process exactly, and there's even more things for the belts rendering-wise that we haven't done yet that also I guess is like the next thing we're like yeah maybe this is a little bit faster but we also haven't tried the general optimization that we haven't finished with conveyor belt street yeah because right now like the conveyor belts are like segmented so we're doing instance drawing for each segment and then the next step is to supplement the whole belt we haven't done that yet and even just the small segments gave us a pretty big significant, performance increase so like we can just assume that yeah segmenting the whole thing would increase it even more so like it's hard to know that's the thing with performance you can't like calculate like we'll get this many milliseconds if we remove this like you have to test you have to do it and test it's science very scientific process a lot of discovery a lot of creative thinking in terms of like how can we shave stuff off and then measure does it work in every case average space is it worth having the code base like this being it's run yeah it runs better but it's [ __ ] impossible to code it now like yeah what are the what are the game design trade-offs of doing this optimization it's like a lot of stuff yeah
