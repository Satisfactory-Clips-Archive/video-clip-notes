---
title: "May 28th, 2021 Dev Vlog Ben Talk: Other optimisations to Constructors"
date: "2021-05-28"
layout: transcript
topics:
    - "features/buildings/constructor"
---
# [May 28th, 2021 Dev Vlog](../2021-05-28.md)
## Ben Talk: Other optimisations to Constructors
https://youtube.com/embed/dyqOMITwLsY?autoplay=1&start=886&end=946

### Topics
* [Features > Buildings > Constructor](../topics/features/buildings/constructor.md)

### Transcript

> cool, and now I can instantly also show off an op another optimization we did, maybe people didn't notice yet but they don't have likes anymore yeah so what we do with the legs now is we only give them legs when it's relevant so if they're on the slope we give them legs some buildings still have legs like the the space elevator obviously because it's they are unique to them they look really good on them too without it it looks a bit weird, the hubs still have them and, what's called again the nuclear reactor I think you still have them so we we have cases where they're still enabled but in general they are disabled and also the constructor has four legs but it means it has the leg and the feet so that would be eight components for just one constructor right again so those are very super easy wins and they also help a lot with loading and saving
