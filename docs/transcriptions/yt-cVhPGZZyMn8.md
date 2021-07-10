---
title: "July 6th, 2021 Livestream Q&A: What does the Object Limit refer to exactly?"
date: "2021-07-06"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [July 6th, 2021 Livestream](../2021-07-06.md)
## Q&A: What does the Object Limit refer to exactly?
https://www.youtube.com/watch?v=cVhPGZZyMn8
<details>
<summary>This question may have been asked previously at least 11 other times, as recently as June 2021 and as early as August 2020.</summary>

* [June 1st, 2021 Livestream Q&A: Can you explain the Object Limit ?](./yt-F1TmvRv7IQ8.md) [https://www.youtube.com/watch?v=F1TmvRv7IQ8](https://www.youtube.com/watch?v=F1TmvRv7IQ8)
* [March 30th, 2021 Livestream Q&A: What's the Object Limit?](./yt-KjV7JMFQ3Is.md) [https://www.youtube.com/watch?v=KjV7JMFQ3Is](https://www.youtube.com/watch?v=KjV7JMFQ3Is)
* [October 9th, 2020 Livestream Q&A: What is the limit?](./yt-Njv_PJT3B2g.md) [https://www.youtube.com/watch?v=Njv_PJT3B2g](https://www.youtube.com/watch?v=Njv_PJT3B2g)
* [October 6th, 2020 Livestream Q&A: What is the object limit and why is it that number?](./yt-VpCuu0aYFw0.md) [https://www.youtube.com/watch?v=VpCuu0aYFw0](https://www.youtube.com/watch?v=VpCuu0aYFw0)
* [September 1st, 2020 Livestream Q&A: Have you thought about implementing a progress bar for how close to the Build Limit we are?](./yt-RyE_hc4huhA.md) [https://www.youtube.com/watch?v=RyE_hc4huhA](https://www.youtube.com/watch?v=RyE_hc4huhA)
* August 18th, 2020 Livestream Build Limit (Part 1): [https://clips.twitch.tv/SplendidAffluentVampireNotLikeThis](https://clips.twitch.tv/SplendidAffluentVampireNotLikeThis)
* August 18th, 2020 Livestream Build Limit (Part 2): [https://clips.twitch.tv/UnusualExquisiteKuduDendiFace](https://clips.twitch.tv/UnusualExquisiteKuduDendiFace)
* August 18th, 2020 Livestream Build Limit (Part 3): [https://clips.twitch.tv/SullenColdbloodedDiscEagleEye](https://clips.twitch.tv/SullenColdbloodedDiscEagleEye)
* August 18th, 2020 Livestream Build Limit (Part 4): [https://clips.twitch.tv/BlitheEnergeticEelPRChase](https://clips.twitch.tv/BlitheEnergeticEelPRChase)
* August 18th, 2020 Livestream Build Limit (Part 5): [https://clips.twitch.tv/GiantGeniusGooseCclamChamp](https://clips.twitch.tv/GiantGeniusGooseCclamChamp)
* August 18th, 2020 Livestream Build Limit (Part 6): [https://clips.twitch.tv/BoxySmallAsparagusSmoocherZ](https://clips.twitch.tv/BoxySmallAsparagusSmoocherZ)
</details>


### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> uh what does the object limit uh refer to exactly one constructor because one object so this is the the confusing thing with the object limit it refers to you object which is not like a physical object or a game object an unreal engine it's an unreal an engine object which is like way programming languages try to like obfuscate how memory works is by referring to massive object you may have heard the term like object oriented languages where they try to like simplify it but how you how you can think of of code um and it's it's essentially a memory object and no one constructor does not equal one object one constructor is could be many objects i don't know the exact number um and they also vary from object to object like maybe you know maybe a beacon is like three objects or maybe two objects or one i don't know exactly and then another constructor could be many objects so uh it's really hard to like to to to to know but something that we sort of tell folks is that like the the number of people that actually hit this object limit is so so few yes like you shouldn't have to worry about it there's unless you're really building some super crazy stuff you really really should not worry about it um and so like you shouldn't have to like don't don't let the object limit impact the way that you play the game unless or do if you want to but you shouldn't need to like you should see a better play as you normally want to yeah and you know we do things on our end to reduce the uh the overhead or the impact that uh objects have on the objective as well yeah so and also the amount of people that hit that object limit that are playing the game vanilla is even smaller uh most people that hit it are using mods to like build way faster and stuff like that and build like humongous things like place i'm thinking i'm talking like placing down like you know half a million foundation blocks and stuff like that um
