---
title: "May 28th, 2021 Dev Vlog Snutt & Ben Talk: Other places Fog Planes are used"
date: "2021-05-28"
layout: transcript
topics:
    - "features/buildings/constructor"
    - "technology/graphics"
---
# [May 28th, 2021 Dev Vlog](../2021-05-28.md)
## Snutt & Ben Talk: Other places Fog Planes are used
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=808&end=887

### Topics
* [Features > Buildings > Constructor](../topics/features/buildings/constructor.md)
* [Technology > Graphics](../topics/technology/graphics.md)

### Transcript

> that was fun so yes uh we are also using this for the fog planes um the fog planes are like the let's make it uh daylight the fog planes are like the the shadow planes that are in front of the inputs and outputs so we can make it look like the items are going properly into the actor instead of just clipping into them but the problem was like the constructor was an example of really object expensive because it had four fog planes even though it was just one yeah yeah it was like four four objects per constructor you need to build a lot of construct just to be able to play the game i guess so we if you have tango structures you have 40 objects that are just those planes that is so ridiculous so that's why these are also in the pool system and it saves a lot of objects for a lot of people so people should be able to build way way more since update 4. cool i believe you also mentioned this in the last video actually you made with chase where this is something that we're going to do in the future here we are in the future the future is the solution cool um and now i can instantly also
