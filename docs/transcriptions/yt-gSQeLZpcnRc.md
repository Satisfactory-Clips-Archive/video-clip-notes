---
title: "October 9th, 2020 Livestream Snutt & Dylan Talk: Instanced Splines (Part 5)"
date: "2020-10-09"
layout: transcript
topics:
    - "coffee-stainers/dylan"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Snutt & Dylan Talk: Instanced Splines (Part 5)
https://www.youtube.com/watch?v=gSQeLZpcnRc
<details>
<summary>This video is part of a series of 14 videos.</summary>

* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 1)](./yt-c6Qy5jzXmqM.md) [https://www.youtube.com/watch?v=c6Qy5jzXmqM](https://www.youtube.com/watch?v=c6Qy5jzXmqM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 2)](./yt-NM5eNwiCX0c.md) [https://www.youtube.com/watch?v=NM5eNwiCX0c](https://www.youtube.com/watch?v=NM5eNwiCX0c)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 3)](./yt-cZgVZMk4zvM.md) [https://www.youtube.com/watch?v=cZgVZMk4zvM](https://www.youtube.com/watch?v=cZgVZMk4zvM)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 4)](./yt-JrWLEvJRhHM.md) [https://www.youtube.com/watch?v=JrWLEvJRhHM](https://www.youtube.com/watch?v=JrWLEvJRhHM)
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
* [Coffee Stainers > Dylan](../topics/coffee-stainers/dylan.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> and the specific thing dylan is working on right now is fixing our instant spline meshes, because spline meshes in unreal engine this aren't instance by default that's something we've done and, have they introduced instant supply meshes or no that's right so we have like parody as well as we can with their instant static mesh right but they do have spline meshes so it's kind of borrowing logic from both, and essentially all our conveyor belts are based on spline meshes which is like a way to twist and turn meshes the models in the game to fit like a curve kind of and that and then rendering them out so our conveyor belts for instance you can tell by like you can twist and turn them and that's essentially the system that dylan's touching right now yeah i'm trying to figure out how they do their how they pass their vertex data for the spline meshes that they have because i think we the issue is arising why they're invisible and is arising because we've switched intentionally to use their their, packaging here because they've changed this up nicely before we declared our own and defined them individually as moving windows around too much as you can see here these parameters but i think we want to pack them down and pick them up the same way because we've combined the macro definitions of ours which used to be separate with theirs so i'm trying to see that let's split oh spline mesh parameters this one i'm looking for and i'm also kind of just hunting and looking for how they do things with theirs to see how we can learning on the job yeah learning on the job this is see yeah it's unfortunately not one of those things that i can just do because i have to see how they're doing but you knew everything about right you know i do this is the one thing it's number one this is the one thing and i just had to stream that yeah so mesh is basically the model in the game so it's, composed of vertices and, combined with those you can like calculate what's supposed to be rendered on screen so it's actually the model, yeah the shape that texture yeah this is a different step on it learning the job is nine percent of being on a job that's kind of true
