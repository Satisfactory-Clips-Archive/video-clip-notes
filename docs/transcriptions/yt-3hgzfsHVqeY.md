---
title: "January 25th, 2022 Livestream Q&A: How am I hitting the UObject limit with 230,000 objects in the game?"
date: "2022-01-25"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [January 25th, 2022 Livestream](../2022-01-25.md)
## Q&A: How am I hitting the UObject limit with 230,000 objects in the game?
https://www.youtube.com/watch?v=3hgzfsHVqeY

### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> someone's saying that they're they're getting the uh they're hitting the u object limit i only have 230 000 items in the game uh so the thing is one item is not one object a u object is the representation of something in the game and items certain items or buildings or whatever may have may be made up of many you objects so it's possible to hit the you object limit with 230 000 items in the game i guess maybe um but there's um there's there's no i don't know if there's a way to really like measure it no there is a way to uh increase that limit but there is no guarantee for any stability um i don't actually know how to do that myself but i think there's a config file you can change i think googling it you'll probably find a solution of how to increase that level there's a reddit post if you google like satisfactory u objects uh that gives you like all the info i think on the wiki as well it even links the maybe the red if we if we could safely change that limit like we would it's not it's not something that we put in we think the games game's better if we have this limit number of objects it's just how the engine works so and do uh if you do change that object limit please know that like it's it's you're kind of on your own because anything can really happen because it has to do with how memory is managed in the game you can even get corrupt save files from changing that number so like save often and save regularly manually if you do change that number just so you guys know
