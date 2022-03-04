---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 1)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 1)
https://www.youtube.com/watch?v=c6Qy5jzXmqM
<details>
<summary>This video is part of a series of 14 videos.</summary>

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
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 13)](./yt-0VtsjQsFzZU.md) [https://www.youtube.com/watch?v=0VtsjQsFzZU](https://www.youtube.com/watch?v=0VtsjQsFzZU)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 14)](./yt-wPV9uZsHLN8.md) [https://www.youtube.com/watch?v=wPV9uZsHLN8](https://www.youtube.com/watch?v=wPV9uZsHLN8)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 15)](./yt-fJRZSb0W8mQ.md) [https://www.youtube.com/watch?v=fJRZSb0W8mQ](https://www.youtube.com/watch?v=fJRZSb0W8mQ)
</details>


### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> but the reason for this is we use a custom component called, instant spline which isn't native to unreal engine they don't have an implementation of it, they do have splines so you can make like and a spline is basically a grouping of curves that create you know nice smooth lines essentially that's a very poor way of explaining that but you can with a mesh component supply mesh component you can put a bunch of mesh meshes along the spline and creates a nice curved from just a single static mesh so like if I was to open up our it also bends the mesh so yeah it lines properly yeah exactly it lines up all the vertices again so like this is what our conveyor mesh looks like and that's it and that's it and then it gets strung along the spline and bent and curved and lines up and looks nice this is the same thing with pipes actually so if I was to build, pipes now which I will do so you can see the the extent of this breaking I don't think this this issue is funny so oh so many things and and you don't know that you're going to get these issues when you upgrade either I mean this one we kind of knew ah damn it you got to turn on the no cost because they don't have this natively in the engine we had to create our own implementation which I did not create so you can see yeah that's the indicator but where's the where's the pipe okay so they're essentially used in the same space they use yeah instant static mesh component and how we do that is we take their existing component which is a instant static mesh and kind of co-opt it into an instant spline mesh so every time we upgrade the engine this is typically the most painful part where we have to take all of their changes to the static mesh code instant static mesh code and convert it into our custom spline mesh instant spline mesh code and this so this is a diff of the two files we have on the left here is their version of the static mesh and then r 423 so this is our 423 upgrade of our spline mesh and these are the cpps so you can see how different they are and we've actually already gone through this and merged all of these and ended up with this version here this is actual code environment and this is what you guys are seeing just now it doesn't work right it works it doesn't crash this was crashing for a long time too and the the last two days before this was fixing some crash books pertaining to these as well but now I'm going to fix it dm yeah so the key key parts of this are the instant spline mesh and our cut we, prepend and fg to all our classes so that's factory game spline mesh so initially when we're going through this we saw that we even like is this gonna work we tried to make it work but we have some solid to do's on here, and this will be this is a lot of code and I there's zero percent chance I will get through all of it like explaining all of it but I'll try to do my best and if anyone has any questions please, please chime in as new we'll probably relay them to me I will feed him yeah so also- I also noticed right just now that I had a typo in the title of the stream I've I've fixed that chat all right calm down this is why we don't have nice things you're you're a poor grammar right poor poor grammar I have poor grammar yes yes yeah so they have made a lot of changes in the last couple of engine versions to the way their rendering pipeline works all for the better in the long run I think but all for the worse when we try to upgrade our custom component the spline mesh here because the changes are significant as I just showed you from the merge differences there that there's a lot of things that have changed and we have to figure out what we need and what we don't need essentially because we actually in a lot of cases we'll just, comment things out completely like this this if zero we keep these here to make merging in the future easier so we can see what was intended from their files so it might like look ugly and like lazy programming but this is actually intentional so that when we take their new version the diff will line up correctly
