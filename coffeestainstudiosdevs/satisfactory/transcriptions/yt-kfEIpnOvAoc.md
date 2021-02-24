---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 10)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 10)
https://www.youtube.com/watch?v=kfEIpnOvAoc
<details>
<summary>This video is part of a series of 14 videos.</summary>

* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 1)](https://archive.satisfactory.video/transcriptions/yt-c6Qy5jzXmqM) https://www.youtube.com/watch?v=c6Qy5jzXmqM
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 2)](https://archive.satisfactory.video/transcriptions/yt-NM5eNwiCX0c) https://www.youtube.com/watch?v=NM5eNwiCX0c
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 3)](https://archive.satisfactory.video/transcriptions/yt-cZgVZMk4zvM) https://www.youtube.com/watch?v=cZgVZMk4zvM
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 4)](https://archive.satisfactory.video/transcriptions/yt-JrWLEvJRhHM) https://www.youtube.com/watch?v=JrWLEvJRhHM
* [October 9th, 2020 Livestream Snutt & Dylan Talk: Instanced Splines (Part 5)](https://archive.satisfactory.video/transcriptions/yt-gSQeLZpcnRc) https://www.youtube.com/watch?v=gSQeLZpcnRc
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 6)](https://archive.satisfactory.video/transcriptions/yt-oyHCEA2k1PM) https://www.youtube.com/watch?v=oyHCEA2k1PM
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 7)](https://archive.satisfactory.video/transcriptions/yt-s-Sa9DA4pDc) https://www.youtube.com/watch?v=s-Sa9DA4pDc
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 8)](https://archive.satisfactory.video/transcriptions/yt-tvqEYd2LI1A) https://www.youtube.com/watch?v=tvqEYd2LI1A
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 9)](https://archive.satisfactory.video/transcriptions/yt-pj50SOLT17Q) https://www.youtube.com/watch?v=pj50SOLT17Q
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 11)](https://archive.satisfactory.video/transcriptions/yt-xAdqOl7aKIE) https://www.youtube.com/watch?v=xAdqOl7aKIE
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 12)](https://archive.satisfactory.video/transcriptions/yt-cMjc0nP-yMM) https://www.youtube.com/watch?v=cMjc0nP-yMM
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 13)](https://archive.satisfactory.video/transcriptions/yt-0VtsjQsFzZU) https://www.youtube.com/watch?v=0VtsjQsFzZU
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 14)](https://archive.satisfactory.video/transcriptions/yt-wPV9uZsHLN8) https://www.youtube.com/watch?v=wPV9uZsHLN8
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 15)](https://archive.satisfactory.video/transcriptions/yt-fJRZSb0W8mQ) https://www.youtube.com/watch?v=fJRZSb0W8mQ
</details>


### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> having that verticality yeah
>
> okay so
>
> this didn't break
>
> which is interesting but
>
> it didn't work either
>
> oh let me take a look at the
>
> file where did you go
>
> make sure i don't have any macros out of
>
> place
>
> [Music]
>
> wait a minute calc this was the thing
>
> would change
>
> just coming out commenting all up on
>
> real engines code no actually i think
>
> this is like so this is a mixture of our
>
> old and new let's see what they're doing
>
> so
>
> use spline form is defined by their uh
>
> shader
>
> when it's um rendering non-instance
>
> blinds
>
> so we can kind of like take a note from
>
> them
>
> but we've also merged some things so
>
> this isn't verbatim what their code
>
> looks like either
