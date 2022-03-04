---
title: "June 8th, 2021 Livestream State of Dev: Dedicated Servers"
date: "2021-06-08"
layout: transcript
topics:
    - "coffee-stainers"
    - "features/multiplayer/dedicated-servers"
    - "retail/steam-store/steam-release"
    - "satisfactory-updates/state-of-dev"
---
# [June 8th, 2021 Livestream](../2021-06-08.md)
## State of Dev: Dedicated Servers
https://www.youtube.com/watch?v=uzSAawwW6EA

### Topics
* [Coffee Stainers](../topics/coffee-stainers.md)
* [Features > Multiplayer > Dedicated Servers](../topics/features/multiplayer/dedicated-servers.md)
* [Retail > Steam Store > Steam Release](../topics/retail/steam-store/steam-release.md)
* [Satisfactory Updates > State of Dev](../topics/satisfactory-updates/state-of-dev.md)

### Transcript

> stream and, yeah state of dev we're working on on the update, we're also working on, stuff, what is it what is the usual thing that people ask about update five is coming fall we're still working on dedicated servers, there's been actually a little bit of development there not that we can say anything yet but we've been making good progress lately with dedicated servers hey, so I'm stoked for that, we you now have someone who is dedicated to the dedicated server aspect yes that dedicated servers right because it is dedicated service requires a lot of things not just the support yes, of it and we actually have someone who's, because it's both you know like the actual dedicated server feature so to speak like being able to for us to be able to build a headless server then there's the biggest aspect for us namely that like all the bugs that are client-side issues and there's a bunch of systems that we've had to rework on client side to be able to like be able to play the game, I actually wrote a steam post about this yesterday or today giving an update sort of and like the the two major issues really with dedicated servers up in this point has really been like the client-side issues and the systems that we've had to implement for two people like support better client-side like both client-side prediction but also like the the there's a ton of critical issues that like you can't progress in the game if you're playing at client side, so those things need to be fixed in order for a dedicated server to make sense at all because otherwise you'll run into issues where you know there's no host to resolve whatever dilemma you're running into so those things need to be taken care of as well, and at least on the non-dedicated servers you can at least play through them or find solutions for those things exactly there's also there's also an aspect to this that we haven't really talked that much about we mentioned it here and there but the when we released the steam version of the game like a big portion of us making the game like for us to be able to release the game on steam was that we kind of needed to be able to support our internal build pipeline for steam which was something that we didn't have in place like whenever we built for our epic version like that was just it we had our build server and that like building the game is quite time consuming actually and it involves a lot of different things because the build server does a ton of stuff for us when it like strips out development stuff and sets it up so it works with that platform that we're uploading it on, so and then do the actual like publication of it so it pushes it to like the server and then we can flip the switch and and make it go live on the store and stuff like that, and there's actually a lot of work that goes into being able to do that and that's a lot of work that we have to do ourselves we're not relying on a service or anything like that to be able to do that I know that there are like certain services out there for like other game engines, where you just like in the editor can be like build for me and it does it on a server, but we had to do that all ourselves and one big portion of that when we built for steam was we needed to be able to support be able to publish both on steam and epic and it's kind of the same thing with the dedicated server aspect of it as well because we need to whenever we make an update to the game we need to be able to push that update out on steam on epic and our dedicated server headless version of the games and if one of these builds fail then they cannot ruin all of them so that's also something that we've spent some time on making sure that that works and yeah good times good times
