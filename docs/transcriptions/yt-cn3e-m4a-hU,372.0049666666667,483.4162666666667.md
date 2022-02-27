---
title: "November 19th, 2021 Video Jace Talk: DirectX 12 is now the default rendering API where supported"
date: "2021-11-19"
layout: transcript
topics:
    - "satisfactory-updates/released/satisfactory-update-5"
    - "technology/directx"
---
# [November 19th, 2021 Video](../2021-11-19.md)
## Jace Talk: DirectX 12 is now the default rendering API where supported
https://youtube.com/embed/cn3e-m4a-hU?autoplay=1&start=372&end=484

### Topics
* [Satisfactory Updates > Released > Satisfactory Update 5](../topics/satisfactory-updates/released/satisfactory-update-5.md)
* [Technology > DirectX](../topics/technology/directx.md)

### Transcript

> we've also made it now that directx 12 is the default rendering api previously the default was directx 11 and of course we have vulcan support as well so you can of course still choose whatever rendering api you want to use but we're now changing it so that directx 12 is the default one the reason for this is that we find that uh from what we can see the directx 12 implementation is like as stable if not more stable than the directx 11 implementation is and generally provides better performance so for the most part if you can run directx 12 it's just basically better that you do now we do do some checks to make sure that your hardware can run directx 12 and if it doesn't we don't switch it to directx 12 we keep it on directx 11. it's possible that this might still cause some issues we've heard from some people that uh they didn't they couldn't support it and it switched anyway um so i just wanna like i've talked about this before here on this channel but i just want to let you guys know again it is possible if you get into a situation where the game is crashing and you're getting errors for a directx do consider trying to change your directx rendering api to 12 or back to 11 to see if that works if the game isn't running at all because you get that crash when it starts up you can use launch options to force a specific rendering api i'm going to leave information in the description below of what launch options you can use to force each respective rendering api and also a link to a resource for how to find out how to use launch options in various launches so launch options are available on the epic launcher and on the steam launcher as well you can also google them information is pretty easy to find but you can use those launch options if you want i'm also going to include information on how to make these changes to your config files i recommend just using the launch options and then like using the launcher options to force whatever random rendering api you want and then making the changes in the options menu and then removing the launch options that's my recommendation and i'm just gonna provide information below so that you can do uh whatever you feel is best okay now there are there
