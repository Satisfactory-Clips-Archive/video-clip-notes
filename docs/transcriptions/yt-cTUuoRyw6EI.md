---
title: "December 7th, 2021 Livestream Q&A: What happens if someone tries to join during an Autosave pause?"
date: "2021-12-07"
layout: transcript
topics:
    - "features/multiplayer"
    - "features/save-system/autosave"
---
# [December 7th, 2021 Livestream](../2021-12-07.md)
## Q&A: What happens if someone tries to join during an Autosave pause?
https://www.youtube.com/watch?v=cTUuoRyw6EI

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Features > Save System > Autosave](../topics/features/save-system/autosave.md)

### Transcript

> what happens if someone tries to join during an auto save pause it doesn't actually pause during the autosave, the game is technically running it's just like held up so it will get kind of queued because of the way the the the game gets paused during that time it's not actually getting paused it's it's that the game loop can't progress to the next frame so that's a different thing than pausing the game because when you're pausing the game the game loop is still running so that's a different thing and if you try to join someone when they're auto saving the game won't like really be able to like handle that incoming request until the save is finished, so the game will like kind of solve that by itself because it's getting queued up because it's the whole thing is getting stopped
