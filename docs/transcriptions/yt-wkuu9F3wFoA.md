---
title: "December 7th, 2021 Livestream Q&A: What contributes to the save file loading / save time?"
date: "2021-12-07"
layout: transcript
topics:
    - "features/save-system"
---
# [December 7th, 2021 Livestream](../2021-12-07.md)
## Q&A: What contributes to the save file loading / save time?
https://www.youtube.com/watch?v=wkuu9F3wFoA

### Topics
* [Features > Save System](../topics/features/save-system.md)

### Transcript

> will contribute to save file loading save time can I make my save load save faster there's nothing you can do really play play the game less get a faster cpu yeah it is cpu bound for the most part stop picking up leaves that doesn't that doesn't really affect it
>
> [Music]
>
>, it does affect it but like yeah ssd I think no I think the biggest part of the save process is still serializing everything which is happening on the cpu so even if you have a fast hard drive it doesn't actually really affect it that much the game might load faster if you have the game on the ssd though because then it's then it's actually loading on the hard drive but like the saving this the part we're actually writing to disk that's a very small part of the of the saving multi-threaded we can't also another topic I would not like to go into because it's not that simple, it is it is serialized to as much as we can we would have to look into other solutions like one thing we can technically do is we could have it so that when we're saving it's, only it's lo only locking the factory buildings, because those are the biggest, issue with I think I don't know if that's true actually it might not be true when I but I'm going to say this anyway, one of the main reasons why saving is like stalls everything so much is because everything is hanging in tandem in the game like one machine output something to a conveyor belt and that convey bill out to something to a splitter and the splitter I put something to another conveyable etc etc so if you were to serialize something you would need to know certain states sometimes where like okay but what if what is my input here and you can't know that until that thing has been processed right which ends up being stalled anyways so even if we did like serialize everything or like paralyze everything it would still stall all the time and you would also run into this parallelization issues that we have to encounter or that we have to account for, that also makes it really difficult to to make the system so I think we just decided at some point that like to make it safe and also a big part of the safe house we wanted to be safe for modding in the future which has been proven because people have made so many save editors and stuff like that, is that we have to construct our save files in a certain way so when we serialize them it won't be an issue and then we decided that we should just do it on a single core because that makes it safer and we can't really like dip on that in certain aspects we can like get around it in certain aspects like it doesn't have to stall the player control and stuff like that but that still means we need to move a lot of logic out of the saving system and add like special cases, but that's one way we could improve it that's just something that we haven't delved into because we haven't we want to like, explore the other options we have with the save system before we would do any like special systems like that, so like the save system can't always get better that's that's the only takeaway that you should get from this like you don't need to understand what I just meant by all this like the safe system can always get better but it's a very complex problem and it just like making it just just paralyze it doesn't solve the problem, and it's not that simple essentially it's the main tldr here, so yeah
