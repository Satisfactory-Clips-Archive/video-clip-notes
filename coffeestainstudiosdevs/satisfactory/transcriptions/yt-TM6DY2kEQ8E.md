---
title: "May 19th, 2020 Livestream Snutt & Gafgar Talk: How Epic / Steam crossplay works"
date: "2020-05-19"
layout: transcript
topics:
    - "features/multiplayer/crossplay"
---
# [May 19th, 2020 Livestream](../2020-05-19.md)
## Snutt & Gafgar Talk: How Epic / Steam crossplay works
https://www.youtube.com/watch?v=TM6DY2kEQ8E

### Topics
* [Features > Multiplayer > Crossplay](../topics/features/multiplayer/crossplay.md)

### Transcript

> no no no just kidding um yeah so that's
>
> that's one aspect like the online stuff
>
> then there's also the cross-play aspect
>
> as to like getting that to work
>
> yeah and that's that's the real
>
> like that's a big topic as well because
>
> of how the different platforms have
>
> support for different things
>
> and for example there is still an
>
> issue that we have are working around
>
> that we hope to solve
>
> in the future i i should i don't know if
>
> how much i
>
> should say but like it's it's
>
> essentially that you can't
>
> if you're don't own an application on on
>
> steam
>
> you can't start uh the steam api
>
> uh with that platform's id it's
>
> impossible you can't do it
>
> which means if you can't start an api
>
> you can't resolve
>
> the state of your friends even you can't
>
> even get your friends list normally
>
> you can do that through other means but
>
> if you get a friend's list how do you
>
> see what game they are in and so on you
>
> need to get their state
>
> and you can't do that unless you own it
>
> on steam
>
> uh and that's like something we have to
>
> work around
>
> uh and there might be solutions that are
>
> really good for it but
>
> but like one solution we are doing now
>
> that is that when you have a session up
>
> and running
>
> you have an id for that session
>
> and anyone that has that id can join you
>
> if you set that option of course um and
>
> that means that
>
> no matter what platform they're running
>
> on as long as they have they i that id
>
> they can join you so you don't need
>
> necessarily
>
> uh the friendly store like their state
>
> you can join them just by knowing the
>
> session and
>
> that is exactly how a dedicated server
>
> would work as well you have the id
>
> of the server and that's how you can
>
> join it
>
> right so does that mean like when if you
>
> want to cross play
>
> you can't really do beyond the epic end
>
> and then like add in your steam friends
>
> it's the other way around or how does
>
> that yeah so
>
> right now when you're if you're using
>
> steam you can just
>
> say hey i want to connect uh my epic
>
> account and then you log into epic
>
> and then you can be on both at the same
>
> time you don't have to own the game on
>
> epic to do that you just have to
>
> log in and that means you can get all
>
> epic friends
>
> and you can get all your steam friends
>
> in one list
>
> the issue is that your epic friends
>
> playing only on epic and doesn't own the
>
> game on steam
>
> will not actually be able to see your
>
> steam presence but they can see your
>
> epic presence
>
> so that kind of will work mostly
>
> seamless for
>
> for most people but there will be cases
>
> where
>
> where if you only own the game on epic
>
> and your friends only own it on steam
>
> then you will not be able to directly
>
> see your
>
> and he doesn't want to have a epic
>
> account
>
> so you can be friends in epic so you
>
> can't like connect
>
> that way you will have to use the
>
> session id you got it
>
> there's a question here on like do you
>
> guys have session passwords with the ids
>
> or
>
> because i assume there's there's author
>
> authentication with the
>
> login within the different or how does
>
> that work right now you have to just set
>
> uh like yours your session to be
>
> uh public er in a way not public but
>
> it's like it's final by a session id
>
> but it must be an exact match and this
>
> you don't have full control of the
>
> session id it needs to
>
> include uh some characters that you
>
> don't actually have control over
>
> ensuring that it's a unique id
>
> and it's not too easy just to randomly
>
> find
>
> and that's all you need to join right
>
> now
>
> like the if if we run problems with that
>
> we'll i
>
> hope we can build on top of that and
>
> uh it's just in general that like the
>
> steam issue with the like you're
>
> logging in on steam maybe there's a
>
> workaround for that as well but
>
> it's uh it's not stuff like that are
>
> certain and there are different
>
> solutions so i
>
> can't really talk too much about that
