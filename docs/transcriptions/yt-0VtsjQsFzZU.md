---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 13)"
date: "2020-10-09"
layout: transcript
topics:
    - "features/buildables/conveyor-belts"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 13)
https://www.youtube.com/watch?v=0VtsjQsFzZU
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
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 11)](./yt-xAdqOl7aKIE.md) [https://www.youtube.com/watch?v=xAdqOl7aKIE](https://www.youtube.com/watch?v=xAdqOl7aKIE)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 12)](./yt-cMjc0nP-yMM.md) [https://www.youtube.com/watch?v=cMjc0nP-yMM](https://www.youtube.com/watch?v=cMjc0nP-yMM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 14)](./yt-wPV9uZsHLN8.md) [https://www.youtube.com/watch?v=wPV9uZsHLN8](https://www.youtube.com/watch?v=wPV9uZsHLN8)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 15)](./yt-fJRZSb0W8mQ.md) [https://www.youtube.com/watch?v=fJRZSb0W8mQ](https://www.youtube.com/watch?v=fJRZSb0W8mQ)
</details>


### Topics
* [Features > Buildables > Conveyor Belts](../topics/features/buildables/conveyor-belts.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> like that's interesting yeah and then we never got around to doing implementing that and then, yeah i've seen this history you've seen this yeah that's kind of weird so that is this okay that's like that's this mesh without the spline doing anything on it yeah and it wasn't it wasn't there before why is it backwards well i'm guessing that would be the default like if the origin it is so the world position and tangent and stuff is all yeah because if you aim at the other one the other left side of that it should be the same position but no it's going to be on the other one know what i mean on the other one like yeah yeah because that's going forward exactly yeah that's what i mean yeah so why does it only show when i dismantle because the dismantle actually applies the material on the the mesh yeah that is oh no it's just always world origin okay that looks like because this is so everyone knows this is zero zero just something to remember yeah so that's the world that's just default transform okay isn't it relative no because it was it's always facing the same because zero zero is is a bit right to where you are well it's its position is relative but it's i'm saying it's a rotation okay it's basically just using, none okay i'm going to take a look at the ush here ish which i apparently only have on one of my desktops if you're wondering why i'm not finding it sometimes okay what's trying to stand on one like the the conveyor belts do work stan they are there and they will transport items they just don't render yeah so i'm trying to fix the rendering portion of it factory get world position is this the one we modified no we want instance position oh wait wait wait a minute so this is under death pass only we're doing something different here bp material effect conveyor build reports no material is set, i don't think that's tied to this issue no actually yeah i've noticed that that is something to do with the order of events with our spline meshes their build effect is totally different from the standard build effect and it i think it creates an actor which creates a bunch of components so i think there's a frame where it's creating the actor that's going to build do the build effect and so it's missing for that frame we should fix that i think that's been there it's i think it's been there a long time for a long time i think that's on poles as well get the same error okay calc slice transform
