---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 11)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 11)
https://www.youtube.com/watch?v=xAdqOl7aKIE
<details>
<summary>This video is part of a series of 14 videos.</summary>

* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 1)](./yt-c6Qy5jzXmqM.md) [https://www.youtube.com/watch?v=c6Qy5jzXmqM](https://www.youtube.com/watch?v=c6Qy5jzXmqM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 2)](./yt-NM5eNwiCX0c.md) [https://www.youtube.com/watch?v=NM5eNwiCX0c](https://www.youtube.com/watch?v=NM5eNwiCX0c)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 3)](./yt-cZgVZMk4zvM.md) [https://www.youtube.com/watch?v=cZgVZMk4zvM](https://www.youtube.com/watch?v=cZgVZMk4zvM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 4)](./yt-JrWLEvJRhHM.md) [https://www.youtube.com/watch?v=JrWLEvJRhHM](https://www.youtube.com/watch?v=JrWLEvJRhHM)
* [October 9th, 2020 Livestream Snutt & Dylan Talk: Instanced Splines (Part 5)](./yt-gSQeLZpcnRc.md) [https://www.youtube.com/watch?v=gSQeLZpcnRc](https://www.youtube.com/watch?v=gSQeLZpcnRc)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 6)](./yt-oyHCEA2k1PM.md) [https://www.youtube.com/watch?v=oyHCEA2k1PM](https://www.youtube.com/watch?v=oyHCEA2k1PM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 7)](./yt-s-Sa9DA4pDc.md) [https://www.youtube.com/watch?v=s-Sa9DA4pDc](https://www.youtube.com/watch?v=s-Sa9DA4pDc)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 8)](./yt-tvqEYd2LI1A.md) [https://www.youtube.com/watch?v=tvqEYd2LI1A](https://www.youtube.com/watch?v=tvqEYd2LI1A)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 9)](./yt-pj50SOLT17Q.md) [https://www.youtube.com/watch?v=pj50SOLT17Q](https://www.youtube.com/watch?v=pj50SOLT17Q)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 10)](./yt-kfEIpnOvAoc.md) [https://www.youtube.com/watch?v=kfEIpnOvAoc](https://www.youtube.com/watch?v=kfEIpnOvAoc)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 12)](./yt-cMjc0nP-yMM.md) [https://www.youtube.com/watch?v=cMjc0nP-yMM](https://www.youtube.com/watch?v=cMjc0nP-yMM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 13)](./yt-0VtsjQsFzZU.md) [https://www.youtube.com/watch?v=0VtsjQsFzZU](https://www.youtube.com/watch?v=0VtsjQsFzZU)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 14)](./yt-wPV9uZsHLN8.md) [https://www.youtube.com/watch?v=wPV9uZsHLN8](https://www.youtube.com/watch?v=wPV9uZsHLN8)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 15)](./yt-fJRZSb0W8mQ.md) [https://www.youtube.com/watch?v=fJRZSb0W8mQ](https://www.youtube.com/watch?v=fJRZSb0W8mQ)
</details>


### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> okay so this is interesting yeah I don't want any of this let's take a look here return variant transform local world so the things that have changed since we changed the spline params I have to make sure that they're all lining up okay and before
>
> [Music]
>
> before I'm in the 423 version I won't do the compare now but we actually had a custom implementation for these two and I'm worried that we're going to have to revert to that, but it was basically we called one function which would call their code if it was their splines and would call our code if it was our splines but now that we're using their data we thought it would be best to try to merge the two and this is essentially just zeroing everything out that we don't use for the instancing that comes with the data so, nice thing is I think let me see I'm googling something real quick I wonder if this will like, break everything I think there's a console command for I've modified the ush file and I think I can read file but I can't remember if there is oh yes the urge file does anyone in chat now if you can what was the thing I want to recompile because I've modified the the, local vertex factory.ush and I think I can force that while running but I don't I think I've just yeah I don't know I mean I can restart the editor but yeah that's what I do hi alert okay, but it might also recompile everything yeah I'm just gonna restart I have done this now that I think about it have you now yeah because I did custom rendering pipeline stuff once and, if you don't do that then it takes years it's like isn't there like recompile shader command something something, well you can't check now because you close the editor I guess yeah let me just there's a force something force recompile yeah I'm restart I'm just gonna restart the other see if this helps at all do
