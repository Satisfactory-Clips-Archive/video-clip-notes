---
title: "July 6th, 2021 Livestream Q&A: Why does the game render items & Belts hidden behind walls even when they're not visible?"
date: "2021-07-06"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "features/buildables/walls"
    - "technology/graphics"
---
# [July 6th, 2021 Livestream](../2021-07-06.md)
## Q&A: Why does the game render items & Belts hidden behind walls even when they're not visible?
https://www.youtube.com/watch?v=uO1QT1SKsZA

### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Buildables > Walls](../topics/features/buildables/walls.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> why does the game render item and belts hidden behind walls even when they're not visible it seems like hiding everything behind the wall has no impact on performance yeah so the way that like uh rendering the stuff on the belts work and we sort of just talked about this a little bit earlier is that they're they're rendered in a sort of like a clever way using instancing so that like rendering the each individual item on the belt is it's it doesn't impact performance in the way that you think it does it kind of just draws them all in one go as opposed to like you've got a thousand separate objects that are being like stored and rendered it it isn't rendered that way and so like simply hiding it behind the wall i don't think is gonna impact it in the way that you think yeah like sometimes i mean the the what's the term for that like there are aspects of the game where like if you put stuff behind walls it will hide the stuff behind the walls because it doesn't need to render it but you know the way like jay said we we instance a lot of stuff which means that stuff is sort of rendered in batches and it's kind of kind of hard sometimes for the game and the the rendering pipeline to sort of know you know whether or not it can render an entire batch or not and if that's the case it will render the entire batch because it's kind of weird if it doesn't if you know it doesn't really make a difference if it renders half of the batch yeah and if you have like cases where say that you have like five buildings and four of those are obfuscated by walls and then one is rendered and it needs to batch all the five buildings then then it's gonna render all the buildings uh and if it was like no most of them are not like you can't see them like ditching that fifth one is gonna be weird but there are cases where that happens um where it does where's the word
>
> [Music]
>
> whatever it's it's complicated the yeah it's it's not it's not like the way that where it is really complicated and the way that it works isn't completely intuitive so like you would think that if i hide it i can't see it then i won't draw it it doesn't really work that way and the reason it doesn't work that way is because in the average case what's actually happening ends up being better um and it's like a very clever way to organize things and sometimes there can be cases where yeah it would have been better to maybe you know split the batch and then render it in a separate way but it's hard to like find those cases and also we have to figure out how to solve that if we do that but it's a really complicated problem um i'm still trying to figure out what the word is is that i believe in you i'm never gonna whatever i'm gonna come up with it like as the stream ends and when you do you tell us oh yeah i better believe it i wanna hear
