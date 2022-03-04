---
title: "June 29th, 2021 Livestream Q&A: In an infinite building game how do you quantify an acceptable performance on standard specs?"
date: "2021-06-29"
layout: transcript
topics:
    - "technology/graphics"
---
# [June 29th, 2021 Livestream](../2021-06-29.md)
## Q&A: In an infinite building game how do you quantify an acceptable performance on standard specs?
https://www.youtube.com/watch?v=Ib023Qb25Pw
<details>
<summary>This question may have been asked previously at least 1 other time, as recently as October 2020.</summary>

* [October 9th, 2020 Livestream Q&A: What do you use to test performance gains?](./yt-YPWIkvRbeHI.md) [https://www.youtube.com/watch?v=YPWIkvRbeHI](https://www.youtube.com/watch?v=YPWIkvRbeHI)
</details>


### Topics
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> in an infinite building game how do you quantify an acceptable performance rate on standard specs when you fix it when you're accepted is good enough this is a this is a good question because we don't know like it's really difficult to to know and also like how people play the game is very different some some build very big factories some go more for like the exploration part the way we do it right now is essentially we have a defined budget that is like how much time can certain aspects of the game run in milliseconds on like low tier and high tier so we are we have or I don't know if we do have it or we are gonna get it but we have like a standard machine at the office that runs like automated tests that do like various things and then people look at that and like oh look how bad the rendering thread is today oh bad bad whoever did something, and then we have a low spec machine that's like less than ideal and then we see like how the game runs on that and then we try to like balance that, but I don't really have a good answer on like what we think is good enough because it's especially not since the game is still evolving and we're still updating the game and and I think I think that the the process is usually kind of we notice certain bottlenecks right yeah and then we target we target those things like what what can we get the most results from yeah, because I think I think at the end of the day there's just gonna be like a but we did our best and that's just kind of it yeah yeah we have to be we have to accept that because there's like there's a good point there because there's there's low hanging fruit that's like oh this is a big bottleneck and it's kind of like the the thing that ben talked about during the lighting thing with the highlighting of, does its mental effect like the way it used to work was that we would replace the material on the building itself, but doing so would mean that at the start of the game it needs to cache a bunch of material instancing on all the the machines and the more machines you have the slower that would take because it needs to do that for the first frame and then once it's done with that it throws that information out because it's set up, and then when you notice that that's like that's a pretty huge gain if we get rid of that, but sometimes it's like we have to re write huge systems and then it's like it's really worth it for to save like a couple of ms, sometimes it's not even certain that you do save because it's very complex sometimes we save on time in areas where we didn't expect to save time and sometimes we do so it's a tricky tricky thing to balance for
