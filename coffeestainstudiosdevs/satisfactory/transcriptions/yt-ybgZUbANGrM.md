---
title: "March 9th, 2019 Livestream Q&A: Weirdest bug you guys fixed"
date: "2019-03-09"
layout: transcript
topics:
    - "features/transportation/vehicles/tractor"
---
# [March 9th, 2019 Livestream](../2019-03-09.md)
## Q&A: Weirdest bug you guys fixed
https://www.youtube.com/watch?v=ybgZUbANGrM
<details>
<summary>This question may have been asked previously at least 1 other time, as recently as February 2019.</summary>

* [February 6th, 2019 Livestream Q&A: What's the biggest bug you guys have seen so far?](./yt-Dtm6xIj-wM4,3623.301698,3734.266666666667.md) [https://youtube.com/embed/Dtm6xIj-wM4?autoplay=1&start=3623&end=3735](https://youtube.com/embed/Dtm6xIj-wM4?autoplay=1&start=3623&end=3735)
</details>


### Topics
* [Features > Transportation > Vehicles > Tractor](../topics/features/transportation/vehicles/tractor.md)

### Transcript

> back what is weirdest bugs you guys yeah
>
> chase
>
> did you have a good one okay okay so i
>
> had about
>
> it's gonna take me a while to explain it
>
> so i'm gonna focus on that oh
>
> how many times you're gonna do that
>
> simon honestly it's a reflection
>
> you know you're
>
> vehicle called a tractor which is a
>
> little square a little just little
>
> tractor right
>
> and we have like a test level that we
>
> have with like a bunch of random objects
>
> that we drive on or whatever
>
> and on that test level there is also a
>
> thing
>
> it's it's a teleporter not saying there
>
> are teleporters not saying there will be
>
> right we
>
> we at one point uh meddled with the idea
>
> of
>
> teleporters and so so that teleporter
>
> was like really old and dodgy was just
>
> on the other side of the map and one of
>
> our guys
>
> found that it was simon simon realized
>
> that if you drive up onto this ramp on
>
> this level with the tractor
>
> stopped got out the tractor just
>
> disappeared and then drove out of the
>
> teleporter
>
> and we're like wait what like what the
>
> hell is going on
>
> and so we kept testing it and we found
>
> if you had to go up
>
> stop at a specific point get out and
>
> then it would and then it would just
>
> drive out a teleporter
>
> or if you stayed in you would just die
>
> and we're like what is going on
>
> that week when i was programming the
>
> vehicles i added a new feature called
>
> camber which is like
>
> if these are the wheels that makes them
>
> turn in and out like that
>
> i added that and then in the code there
>
> there was
>
> unfortunately a divide by zero uh error
>
> which means you know you could have a
>
> number divided by zero and then it
>
> becomes infinity
>
> and then that that value was then used
>
> as force on the vehicle so the for the
>
> vehicle got
>
> infinite uh forces applied to it so it
>
> grew
>
> to be infinitely big and when it grew to
>
> be infinitely big
>
> it hit the teleporters hit the
>
> teleporter's trigger box
>
> and then it it got re reset back down to
>
> there
>
> all the forces were clamped again and it
>
> just drove out of the teleporter
>
> classical saturday night
>
> did you crash no no no no no he didn't
>
> yeah no he's just he's kidding around
>
> you know
>
> that's what you get when you when you uh
>
> hold a nut for too long apparently the
>
> game doesn't
>
> did you get a fun call sack though uh
>
> did you did you
>
> remember to uh fill in the the the field
>
> i just did it now and explain what you
>
> did sometimes
>
> and your comment feels like i was
>
> telling a funny story i was just
>
> standing there in all caps i was just
>
> standing in there snoop was building
>
> foundation see me
>
> thank malone's gaming i really
>
> appreciate it it was something to do
>
> with the
>
> skeletal best skinned mesh component
>
> refresh
>
> bone transform yeah okay
