---
title: "September 6th, 2022 Livestream Q&A: Can you making saving incremental in the background?"
date: "2022-09-06"
layout: transcript
topics:
    - "features/requested-features"
    - "features/save-system/autosave"
---
# [September 6th, 2022 Livestream](../2022-09-06.md)
## Q&A: Can you making saving incremental in the background?
https://www.youtube.com/watch?v=TLz62bpBmjI

### Topics
* [Features > Requested Features](../topics/features/requested-features.md)
* [Features > Save System > Autosave](../topics/features/save-system/autosave.md)

### Transcript

> can you make saving incremental in the background so kind of ties into this a little bit because the saving ish thing as well is the reason why we have it on the game thread at the moment which means it pauses everything is because that is the safest route that we we see at the moment we can make it, so that you know the game can like maybe machines pause or something while we're doing it because that is a huge operation like the serialization operation, and technically we could make it so that you could still like walk around and jump around and interact with animals and stuff like that but that is very risky because making a save system is very difficult making a safe safe system that also ties into like real time application it's also very tricky especially when it takes so long for our serialization process to go through and there's so many likes again so many sequential things you know like we can't paralyze that either because they tie into like one another and you don't know the state of things so it's not a good like thing to to actually run in parallel it has to be sequential, and we've just opted to like just pause everything when we do the same thing just because otherwise you can run into really ugly like corruption issues on your save files that you sometimes can't catch like un until you try and load it, so that that is really the main thing like we don't want save files to be corrupt that's the main reason why it is that is right now it is possible to to go in a different route but it's a lot of work and we will see if we have time for that in the future essentially so it is it is what it is kind of, if we could fix it then we would love to but it is such a scary thing such a scary undertaking at the moment so yes just download more cpu kind of more cycles baby we should yeah we should just have it so that we have we're running like different cores or different threads all the time so it looks like the game is doing a lot of stuff, and then we could be like oh the game's running so slow and can be like oh we got a fix for that and we just remove that and suddenly the games runs a lot faster and then it goes back and then it goes in a circle because then people are going to complain again like oh it's not using enough threads but the game is running faster and then we do that again and rinse and repeat baby
