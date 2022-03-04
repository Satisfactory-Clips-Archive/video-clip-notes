---
title: "January 25th, 2022 Livestream Q&A: Why does the game lag during a save, it's especially jarring on Dedicated Servers?"
date: "2022-01-25"
layout: transcript
topics:
    - "features/multiplayer/dedicated-servers"
    - "features/save-system"
---
# [January 25th, 2022 Livestream](../2022-01-25.md)
## Q&A: Why does the game lag during a save, it's especially jarring on Dedicated Servers?
https://www.youtube.com/watch?v=I6kMEiZYYRQ

### Topics
* [Features > Multiplayer > Dedicated Servers](../topics/features/multiplayer/dedicated-servers.md)
* [Features > Save System](../topics/features/save-system.md)

### Transcript

> why does the game lag during a save is especially jarring on dedicated so that's probably like maybe two too big of a like subject to go into, this late in the stream but tldr it has to do with, that all your factory like everything is like linear or whatever so like when we're saving we need to pause everything to make sure that the states are like in a correct way when we're saving and if we were to run that while the game was running sort of how most games do it then we would kind of run into issues where if you have a big save and you have like a lot of stuff going on, it can run into like states where it's like where it's saving a state but it actually moved on to the next one and they get like weird, race conditions so we have to kind of pause the, the factory logic while we're doing it and that's the main reason why we're doing that why the it lags like that, so it pauses the game thread so that's the main reason
