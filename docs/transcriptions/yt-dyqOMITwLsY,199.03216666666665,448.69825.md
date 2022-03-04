---
title: "May 28th, 2021 Dev Vlog Q&A: Can you give a quick explanation of how the system for Lights works right now?"
date: "2021-05-28"
layout: transcript
topics:
    - "environment/creatures/lizard-doggo"
    - "features/buildables/conveyor-belts"
    - "features/buildables/lights"
    - "features/possible-features/decor"
    - "satisfactory-updates/seasonal-events"
    - "technology/graphics"
    - "technology/unreal-engine"
    - "technology/unreal-engine/distance-fields"
---
# [May 28th, 2021 Dev Vlog](../2021-05-28.md)
## Q&A: Can you give a quick explanation of how the system for Lights works right now?
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=199&end=449

### Topics
* [Environment > Creatures > Lizard Doggo](../topics/environment/creatures/lizard-doggo.md)
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Features > Buildables > Lights](../topics/features/buildables/lights.md)
* [Features > Possible Features > Decor](../topics/features/possible-features/decor.md)
* [Satisfactory Updates > Seasonal Events](../topics/satisfactory-updates/seasonal-events.md)
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Distance Fields](../topics/technology/unreal-engine/distance-fields.md)

### Transcript

> right cool cool so can you just give like a quick, explanation of like how light this like the system for lights works right now i haven't anything set up to show so i'm first gonna show problems with light i'm totally not using our first of april settings so here we have a beautiful statue and these are like 50 lights overlapping so if we show our performance it's, it's kind of that we're running at less than 30 fps even though not much is going on here that looks great so the yeah i know i love the floating floating peeps, so the first thing we did an engine upgrade to 25 i think which gave us a nice future which is the rendering threat the rhi threat
>
> [Music]
>
> which gives us tons of performance back already the rhi stands for rendering hardware interface which is epic solution for different rendering apis and with the engine upgrade we are allowed to use in separate fret for this so partially the work is offloaded to a separate threat instead of only on one fret so this is acceptable now so now we can go to stage two of the explanation so the second thing we did with light is normally you would use inverse square falloff which makes the light look pretty realistic but the problem is they lose a lot of intensity so instead of that we are using no falloff so the light is the same strength as the beginning as the end which allows us to have the right distance for the light so they are way less performance impactful and they need to overlap way less to get intensity that you would desire right so they're not like realistic in the sense that most other lighting in the game is but they kind of need to to make sense for the users yes and here we see the example how it works with a ceiling light so we slap a cookie cutter on it, called a light function and then we cut out the square so it's technically this light but we just cut out the other parts right and then the biggest issue with the light is shadows so let's go to the shadow part so we have three options, no shadow casting which looks disappointing there's absolutely no shadows from anything the second option is cascaded shadow mapping, this is the classic way of doing it we have been doing that ever since i don't know 2005 probably it's it's expensive because just imagine the light being a camera it looks what is visible and then makes a depth map and projected shadows on the world that way so the more objects the light is hitting the more expensive the shadows will get which is absolutely not ideal in an infinite builder game so and then we have the last option which is distance field based lights, shadows, it has some downsides our conveyor belts are not shadowed unlike in this case there there is shadows from the conveyor belt that's why we use the mix solution for the directional light and as you can see some shadow artifacts will pop up and that's because distance fields are technically a 3d rep 3d texture of the mesh itself so if i quickly eject this is the distance fields for those objects they look a bit of funky but it's easier for the gpu to calculate it because it's just direct information there it doesn't really need to do much curling because it's it's gpu to gpu data but it's like 25 to 50 faster especially with the rendering, the error hia threat, that made it even more fast, so yeah that's why we're using that right and like so so you mentioned that
