---
title: "May 19th, 2020 Livestream Snutt & Gafgar Talk: What we had to do in order to support Multiplayer on Steam"
date: "2020-05-19"
layout: transcript
topics:
    - "features/multiplayer"
    - "features/multiplayer/crossplay"
    - "retail/steam-store/steam-release"
---
# [May 19th, 2020 Livestream](../2020-05-19.md)
## Snutt & Gafgar Talk: What we had to do in order to support Multiplayer on Steam
https://www.youtube.com/watch?v=tzQZ1akwzzM

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Features > Multiplayer > Crossplay](../topics/features/multiplayer/crossplay.md)
* [Retail > Steam Store > Steam Release](../topics/retail/steam-store/steam-release.md)

### Transcript

> all right fantastic, so let's start let's talk a little bit about, the the work that's been put in on the in the steam version, because I think a lot of people have been confused as to like what we've actually had to do to be able to support multiplayer on on steam, and it's it's not just like one thing we've had to work on it's many things so like could you give me a like roundup of the things that we've had to do like between now and when we started working on being able to run the game on steam, yeah so first of all to set the scene a little bit here we had a multiplayer solution but it's been growing and kind of not being prioritized enough throughout a long like the whole development, and it kind of consists of many different parts on top of each other and we also had a kind of hacky way to work around the feature, called sessions we never actually had sessions, and to get proper multiplayer working especially crossplay but also even just proper multiplayer working, we want sessions like that's necessary so we need to start rebuilding stuff to actually use sessions and that means even part of the ui need to be reworked to handle kind of like a delay of querying and like receiving data that is inherent to multiplayer if if you work around stuff you need to hack solutions maybe you have the buffer you can do stuff instantly but as soon as you start processing like querying more stuff from the server you need to build in more delays in like ui stuff to handle this it's short it's like the ping kind of delay but it's, it's still a delay, it's not the same frame, and just doing that is a lot of work than like we have been merging all those kind of systems I mentioned into one system to make it, much more manageable for the future like continuing in development and this will help a lot with dedicated servers well like you mentioned before that there's not been a lot of progress on dedicated servers but I actually would claim that there has been a lot of progress on that front to be just indirectly from making this session system change because flashes is what the dedicated service needs, in a way to identify a session through an id instead of like just finding a friend because the dedicated server will not be on your friend list you will have to have other ways of joining a session that is not your friend list and that we didn't have before cool so we've essentially been working on dedicated services that are working on the steam release got it is that how it came across no no just kidding
