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
<details>
<summary>This question may have been asked previously at least 10 other times, as recently as March 2021 and as early as August 2020.</summary>

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

> can you explain the object limit so the object limit is um it's related to unreal engine's garbage collection so it's just a thing that keeps track of all the objects and helps clean them up in memory and all that kind of stuff right um and what what an object is it's not like an item in game right an object is an unreal engine game object right and and this doesn't really make too much sense to a player but if you're a developer you know like so so there could be like you know an object could be a like i think a foundation could be an object but sometimes like one single building can be made up of multiple objects so like a constructor i think historically had like four or four four or seven or something like objects in one object right so like that's and so we've done things to help like optimize that but that's what the object limit is and so the the the max limit there is just how many of those unreal engine game objects can we keep track of at a time
