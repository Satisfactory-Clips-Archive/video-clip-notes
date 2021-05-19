---
title: "May 18th, 2021 Livestream Q&A: What's so hard with implementing Train hit box?"
date: "2021-05-18"
layout: transcript
topics:
    - "features/multiplayer"
    - "features/transportation/trains/train-signals"
---
# [May 18th, 2021 Livestream](../2021-05-18.md)
## Q&A: What's so hard with implementing Train hit box?
https://www.youtube.com/watch?v=lD9c8z6BYJI

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Features > Transportation > Trains > Train Signals](../topics/features/transportation/trains/train-signals.md)

### Transcript

> so what like what's so hard with implement implementing train hitbox so there it's it's easy so this is like another one of those things where if you think about it that way it seems really easy because it is i mean we could just put collision on the trains right but then but what happens when they collide not only that but what happens if trains can collide how do you handle uh trains that are supposed to then like pass each other like multiple trains on a single line um i guess there should be signals or something like that and if that's the case how do they work now how are they supposed to function in the game what's this experience going to be like so it's it's not about just simply putting a hitbox on a train it's everything like when you make one designed decision with a game it touches a lot of different things and that has a knock-on effect so you have to do a lot of things to justify even just to justify hitboxes on a train yeah right so it's it's not as simple as just that one thing and as and and as as the developer uh and i've mentioned this many times before as a developer as opposed as opposed to say like a modder for example as a developer we have the responsibility to make everything work and justified working together in a straightforward and simple manner uh for the user um and so we can't just leave necessarily like half-finished things in and top it all off the game is also a multiplayer so suddenly that collision also needs to be maybe handled on client and how do you handle that um and stuff like that because a lot of times a lot of times when you see things happen on client it's all like quote unquote fake and it's like simulated because the client doesn't know their exact state and they can't know all the updates of states all the time that's something that happens a lot with vehicles where the client will always try to predict where things are going but it doesn't always know so like just adding a collision there might not just work on clients sometimes sometimes you need to simulate things and how do you then resolve when the client has simulated in one way but something else happened on the server and the server tells the client like hey actually i'm over here now like how do you handle that so it's it's tricky
