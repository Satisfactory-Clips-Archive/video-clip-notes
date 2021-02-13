---
title: "January 22nd, 2020 Livestream Snutt & Jace Talk: NAT"
date: "2020-01-22"
layout: transcript
topics:
    - "features/multiplayer"
---
# [January 22nd, 2020 Livestream](../2020-01-22.md)
## Snutt & Jace Talk: NAT
https://www.youtube.com/watch?v=4WFbYbEegN4

### Topics
* [Features > Multiplayer](../topics/features/multiplayer.md)

### Transcript

> nat problems uh i don't know if you've
>
> done any more work
>
> on them the dedicated servers will fix
>
> them if you use dedicated servers
>
> hopefully uh yeah hopefully
>
> um but without that i can't remember if
>
> we've done we could talk about
>
> matt in general like why is that an
>
> issue for some people because like
>
> if like you might have seen or
>
> experienced yourself that like sometimes
>
> it's really hard to connect
>
> or maybe you've never been able to
>
> connect and stuff like that uh
>
> and it's like one of the hardest part of
>
> any networking game
>
> is because we're using um
>
> oh what is the protocol called it's
>
> not t uh tps or tsp it's uh
>
> uh i'm like blanking out i just
>
> work with this every day and whatever
>
> udp udp thank you so udp is like a
>
> faster protocol to send data
>
> but it's also like if you just send like
>
> a bunch of transmissions to someone
>
> uh they have to like open their ports
>
> and everything
>
> behind the router if so if they're
>
> behind a router they have to like open
>
> ports to allow like you sending them
>
> data and that's the hardest part of like
>
> connectivity is the fact that like
>
> computers don't want you to open ports
>
> unless you're sending some data first
>
> so there's like a lot of tricky ways to
>
> like try and like
>
> get the router to to allow people to
>
> connect uh
>
> it's a it really is and it's
>
> really frustrating and there's like
>
> we've implemented a few
>
> um things that will mitigate that
>
> but obviously like we're not catching
>
> every single case yet
>
> uh but rest assured that we we know
>
> about it
>
> uh we are looking into ways to get more
>
> people because like obviously we want
>
> everyone to play
>
> and it's a cons like it's a thing that
>
> we just have to work on
>
> all the time like it was the same thing
>
> when i used to work on different
>
> multiplayer games so the same thing like
>
> some people just have not issues
>
> and and the really unfortunate thing is
>
> like sometimes
>
> it's your isp that's messing up for you
>
> because like you can have the issue
>
> where like if you have a router behind a
>
> router
>
> which like not most people have but like
>
> it can happen in certain situations
>
> sometimes it's just like the your isp is
>
> like not forwarding
>
> uh your ip address to your router
>
> because they're like ah this is scummy
>
> um so like there's
>
> it's just such a complex like issue
>
> um and there's so many ways like it can
>
> go wrong and stuff
>
> load decapo has an interesting helmet
>
> there maybe we could i don't know
>
> like you know more about this than me
>
> but udp is sessionless you guys could
>
> start a tcp tunnel the transit protocols
>
> once you get a reply
>
> yeah it's the same issue though because
>
> like you can establish connection
>
> through
>
> to through tps and earlier through tpc i
>
> can't talk
>
> you establish a connection there right
>
> and you say like all right let's talk on
>
> this protocol and then you start the
>
> first transmission and then router's
>
> like nope
>
> that's not i really can't allow that yet
>
> this is that's how youtube works
>
> yeah you visit elizabeth's special
>
> because youtube
>
> keeps the tcp connection going i think
