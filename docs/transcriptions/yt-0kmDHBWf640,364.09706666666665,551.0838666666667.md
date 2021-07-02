---
title: "November 27th, 2020 - Jace Talk: Per-instance Custom Data"
date: "2020-11-27"
layout: transcript
topics: 
    - "technology/unreal-engine"
    - "features/paint"
---
# [November 27th, 2020 Upcoming Engine Upgrade // What is it and why?](../2020-11-27.md)
## Jace Talk: Per-instance Custom Data
https://youtube.com/embed/0kmDHBWf640?autoplay=1&start=364&end=552
### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Features > Paint](../topics/features/paint.md)

### Transcript

> this next one's really cool and i've
> tried to explain this and it's super
> hard to explain so i'm gonna do my best
> i i hope everyone can understand it uh
> and this is her instance custom data and
> i think this is amazing first of all
> the first thing you need to know is what
> an instance is and an instance is just a
> copy so if you build two constructors
> you have two instances of a constructor
> right so they're just copies
> and where the big win is here is on the
> rendering side of things
> renderers are really good at doing the
> same thing over and over
> without interruption or switching tasks
> so what you want to do is when you have
> all your
> constructors built for example you want
> them all to be instances or you want
> them to be considered instances by
> your renderer so that it will take
> constructor data
> what it needs to draw a constructor and
> then it'll draw one
> and then it'll go there's another one
> it's the same thing all right goes
> little dj khaled on our ass
> all right it's like there's another one
> it's a constructor i already have that
> data we'll draw it and then just draw
> all the constructors then throw that
> away and then move on to the next next
> task
> what you don't want is uh for it to see
> two different constructors and think
> that they're different things
> therefore treating them as different
> tasks therefore requesting the same data
> over and over again now this can happen
> when
> let's say you paint them a different
> color with the color gun
> the way we added the color gun into the
> game is we had
> a separate material on
> each unique object for every color in
> the color gun so there are 16 colors in
> the color gun
> every single unique object every
> different kind of wall
> foundation had 16 materials on it
> one for each slot of the color gun so
> that when you paint it
> it will use the the appropriate material
> that you had selected in your color gun
> now to you and me we still see the
> constructors as instances they're still
> copies
> they're the same thing they just look a
> little different the renderer sees
> two constructors with different
> materials on therefore
> different objects so it won't draw them
> one after the other
> it will separate them into tasks now
> that we can use per
> instance custom data or primitive data
> on each
> constructor if we keep going with this
> example it means we can just put
> one material on every constructor and
> have the renderer look at that
> that data that custom data on each
> instance as it draws them
> and put it into the material and then
> draw so basically it means
> we can draw all the constructors without
> being interrupted
> and then move on to the next thing and
> draw all of those without being
> interrupted even if you use different
> colors between them this also adds
> [Music]
> another really big thing that isn't
> going to be in this upgrade but will
> come in the future
> and that is we had a 16 color color
> palette on the color gun before
> because that was just a limitation we
> imposed on ourselves but if we
> only need to use one material per object
> and the custom data
> is on the object then that data could
> just be a color it could be any color
> and that means you could have infinite
> colors
> so this one thing gives us a massive
> performance increase
> and it's going to allow us to expand
