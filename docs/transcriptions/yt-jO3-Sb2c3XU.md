---
title: "September 27th, 2022 Livestream Q&A: Why not pause when I open the menu?"
date: "2022-09-27"
layout: transcript
topics:
    - "features/multiplayer"
    - "features/unplanned-features"
    - "technology/user-interface"
---
# [September 27th, 2022 Livestream](../2022-09-27.md)
## Q&A: Why not pause when I open the menu?
https://www.youtube.com/watch?v=jO3-Sb2c3XU
<details>
<summary>This question may have been asked previously at least 1 other time, as recently as December 2021.</summary>

* [December 7th, 2021 Livestream Q&A: Is that why the game doesn't pause when you press the escape key?](./yt-QVt37vGwEwg.md) [https://www.youtube.com/watch?v=QVt37vGwEwg](https://www.youtube.com/watch?v=QVt37vGwEwg)
</details>


### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)
* [Features > Unplanned Features](../topics/features/unplanned-features.md)
* [Technology > User Interface](../topics/technology/user-interface.md)

### Transcript

> why not pause when I pause the menu the main reason for that is because the game is sort of always online because, if you want seamless if you want to the ability for people to seamlessly be able to join your game then we need to set it up so that it's it's creating an online session, when you start the game essentially and it is possible to make it so that like if there's no one in your session and you pause and you open the menu the game can be like checking like hey is there anyone in session no then I can pause, but the bad thing with doing it that way is that then you create a bunch of case edge cases for when the game should be on pausing so but what if you pause the game someone just joined or just joined just as that happens because of how you know Internet isn't, you know having things running in parallel means that you can run into race conditions, so you have to account for all those cases so while we're in Early Access we've just decided that we shouldn't focus on that for now because that could be a potential thing that's just like too much work to maintain just having the game not just having it so that the game doesn't pause just means that it makes it easier in that case so you're just losing out a feature instead of having a bunch of bugs so, so that's why we don't have pause in the game at the moment and eventually in the future we may add like that functionality so that we can actually distinguish, that feature set but that's a lot of work for something that not everyone might notice, or might want, or make sense so you know we have to sort of decide between either doing that or adding like you know a new feature to the game so it's always that like Balancing Act that we run into but- I mean it makes sense or it doesn't make sense like I'd I'd like the feature too like the so that it actually pauses the game, because there's no there's a couple of games where it does make sense that it doesn't pass like for instance in in camera the names but there's a bunch of games where like you can get like attacked and stuff like that you know like in Dark Souls, and that's supposed to like keep you on your toes all the time so you never know when you're being invaded etc etc getting killed by a spider in a pee break is a is a feature for sure if you open up the console you can pause using the console command pause, so you can pause the game as it is right now this is a bit tedious
