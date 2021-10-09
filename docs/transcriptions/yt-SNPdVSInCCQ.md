---
title: "March 23rd, 2021 Livestream Q&A: Object Limit, any chance to display how much is left somehow?"
date: "2021-03-23"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [March 23rd, 2021 Livestream](../2021-03-23.md)
## Q&A: Object Limit, any chance to display how much is left somehow?
https://www.youtube.com/watch?v=SNPdVSInCCQ
<details>
<summary>This question may have been asked previously at least 2 other times, as recently as November 2020 and as early as September 2020.</summary>

* [November 10th, 2020 Livestream Q&A: Is there a debug command to see how many Objects you are using?](./yt-3Tht0Ap0S8c.md) [https://www.youtube.com/watch?v=3Tht0Ap0S8c](https://www.youtube.com/watch?v=3Tht0Ap0S8c)
* [September 22nd, 2020 Livestream Q&A: What is the Object Count Limit, and how can we tell in our own game?](./yt-gMq-fPCqGWQ.md) [https://www.youtube.com/watch?v=gMq-fPCqGWQ](https://www.youtube.com/watch?v=gMq-fPCqGWQ)
</details>


### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> object limit any chance to display how much is left somehow uh not really the the common misconception about the object limit is that people think that it's like the number of objects that are placed in the world but this is a memory thing so you know placing a foundation has a smaller object you object imprint in memory than placing a constructor has um and it's not simple to explain it because memory in programming is is very complex uh it's not just like a lot of people often like describe it as like it's a it's an array of of of um ones and zeros that's memory no that's not exactly how it works uh because they're there's like memory caches and and setups for how they're loaded and stuff like that but uh the system that handles all that has a limit in unreal engine and uh there's not much we can do about it uh we can optimize for it but there's always going to be a limit um and you can even load a save file that crashes due to the object limit you can you can sometimes load that save file and sometimes you can based on what's going on in the game at that point um so kind of hard to it's it's hard to explain we're optimizing for it um and maybe in the future it will be a bit better but there's all there'll always be like a limit to it
