---
title: "March 30th, 2021 Livestream Q&A: Will Conveyors ever get collision against each other or can I continue my chaos?"
date: "2021-03-30"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/physics"
---
# [March 30th, 2021 Livestream](../2021-03-30.md)
## Q&A: Will Conveyors ever get collision against each other or can I continue my chaos?
https://www.youtube.com/watch?v=AwICAUMlVaI

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Physics](../topics/technology/physics.md)

### Transcript

> will conveyors ever get collision against each other or can I continue with my kos I mean even if we add collision any built conveyor belts should still function like they they won't disappear or anything like that- I don't know we've kind of always liked the fact that conveyor belts specifically don't have collision against one another they have to some degree I think there's some there's some limit to it I can't remember exactly what it is but you can totally like slice them and clip them into each other and slice them around and stuff like that, but I don't know what the plan going forward is honestly- I don't think we're gonna change that because the the reasoning has always been and it- I guess it's kind of like counter counter-intuitive in the stance that we have against like you know foundations because foundations have collision why can't we just remove that the same way we do with with conveyor belts but the the reasoning we've always had with conveyor belts was that the reason why in the beginning we didn't have collision was because it was tricky when you're creating a spline to create like collision for that so we just skipped it for now and think we'll do it later but then we also kind of realized that it's kind of fun for people that don't care about the clipping and aren't annoyed by that because the people that care about clipping and want to look fancy they will build it so that they don't clip they they will avoid clipping whereas people that don't care they can still do it so we like that people have had that option until now to be able to like you know pick and choose kind of what they want, and I guess that stands kind of like get a little bit challenged now with the foundations where people really dig the fact that you could clip the the downward ramp once, and then now we're taking the stats like no we want collision on the ramps on the, on the, foundations the thing about the foundation so that the foundations are a problem with the like memory limit and stuff like that you can't build we don't want you to build too many and collision is kind of the way our way of stopping you doing that it's kind of weird like we need to the game kind of needs you to limit a bit so that you don't hit the the limit too fast and that's kind of one of the reasons why we have collision on foundations and don't want to give that up is because we we don't want you to to get stuck on that but also like if you weren't able to clip foundations inside themselves like when you build foundations you run into issues where you build foundations inside foundations and stuff like that there just needs to be a limit somewhere, and it kind of sucks because we really like the way people utilize the fact that you can't clip and stuff like that it makes it so you have much more freedom so it really is a sucky situation for us because we like we kind of want to go both paths you know but we can't up the limit because the limit isn't set by us it's set by an engine we can only optimize for the limit
