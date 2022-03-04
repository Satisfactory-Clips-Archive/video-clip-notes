---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 12)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 12)
https://www.youtube.com/watch?v=cMjc0nP-yMM
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
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 13)](./yt-0VtsjQsFzZU.md) [https://www.youtube.com/watch?v=0VtsjQsFzZU](https://www.youtube.com/watch?v=0VtsjQsFzZU)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 14)](./yt-wPV9uZsHLN8.md) [https://www.youtube.com/watch?v=wPV9uZsHLN8](https://www.youtube.com/watch?v=wPV9uZsHLN8)
* [October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 15)](./yt-fJRZSb0W8mQ.md) [https://www.youtube.com/watch?v=fJRZSb0W8mQ](https://www.youtube.com/watch?v=fJRZSb0W8mQ)
</details>


### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> that's an interesting to do look at that, our parameters maybe yeah yeah maybe and this was the that looked like a really old comment oh that was to do 425 was it okay spline mesh no that's not where we define that oh wait we don't have the did one part of that what is it the instance splined up it stands spline srv we didn't have that defined okay that's good oh this is a funny account some of these parameters functionality says this is totally new verify like a I guess yeah what have they done okay so that was definitely missing but that's not what it was complaining about because that one yeah yeah you fixed an error that's going to creep up later yeah that's like a future future fix yeah but unfortunately not the one yeah so this is that this is here I don't know why it really like I'm okay well actually let's do this now it's mandatory it should catch it earlier and really complain and not just kind of fail later all right compiler it's inspiring but then spline buffer is not, it's blind buffer parameter no yeah no it's vertex fetch yeah there we go that's the one I'm looking for because it's a vertex fetch now let's see if it comes you just are really missing out on a really intense compile process here
