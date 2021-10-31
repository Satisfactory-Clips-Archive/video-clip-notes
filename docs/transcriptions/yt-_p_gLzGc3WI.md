---
title: "September 14th, 2021 Livestream Snutt & Jace Talk: Vehicle obstacle handling"
date: "2021-09-14"
layout: transcript
topics:
    - "features/transportation/vehicles"
    - "features/transportation/vehicles/autopilot"
    - "satisfactory-updates/released/satisfactory-update-5"
    - "satisfactory-updates/teasers-trailers/update-5-teasers"
---
# [September 14th, 2021 Livestream](../2021-09-14.md)
## Snutt & Jace Talk: Vehicle obstacle handling
https://www.youtube.com/watch?v=_p_gLzGc3WI

### Topics
* [Features > Transportation > Vehicles](../topics/features/transportation/vehicles.md)
* [Features > Transportation > Vehicles > Autopilot](../topics/features/transportation/vehicles/autopilot.md)
* [Satisfactory Updates > Released > Satisfactory Update 5](../topics/satisfactory-updates/released/satisfactory-update-5.md)
* [Satisfactory Updates > Teasers & Trailers > Update 5 Teasers](../topics/satisfactory-updates/teasers-trailers/update-5-teasers.md)

### Transcript

> uh we also added like a little bit of obstacle handling so if it starts running into stuff it will try to like figure out like okay how can i get out of this situation um now this implementation we've done is sort of like a naive implementation so it won't like recalculate the whole route like if you if you set up a route and and you and you start like building factories in the middle of that route it's not gonna like automatically figure out like oh okay i need to go around the whole factory uh it's still gonna like run into stuff and try and like solve it um so that's one thing you can take into consideration and if it does happen to run into an issue where you know the truck runs into something and it can't like solve it then we've also introduced something that's called ghosting which is uh essentially nano machines nano machines that uh for example if your uh explorer gets stuck off a cliff yeah another bean loft city nani machines yeah oh that's so good nani yeah so then uh the truck will uh figure out a way magically to find its way back to the path and uh we will take no questions about this this is science uh don't worry about it it's all good fixit does not promote those who have questions or you know their own start developing their own thoughts exactly it's a one way to the bottom of the barrier follow the intended path um no like it is it is it is a little weird um and it's not like quote unquote realistic but like there's a ton of stuff in this game already that's not realistic so like i don't know where you set the bar or put the boundary whatever um but like the important thing when we made the system is really that we want trucks to be deterministic and like consistent and like reliable and uh like this is really the last sort of ditch effort to maintain that really so that um trucks are reliable so uh you know yeah and and and like people people who don't want this to happen if you don't want this to happen in your game re-record your path so that it doesn't do it yeah you know that's that's basically it right so if if your vehicles keep falling off cliffs and have to down a machine and you don't like nano machines re-record the power so it doesn't fall off a cliff but until you do at least it will keep working yeah and we think that's like a fine trade-off yeah just just like just like with soft clearance that we showed before right it does it's not very realistic to have you know conveyor belts that go directly through buildings um and if that matters to you you know you'll just rebuild your conveyor belt so that they don't clip right but if you don't care then just go and do whatever you want yeah exactly
