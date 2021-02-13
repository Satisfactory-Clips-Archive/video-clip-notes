---
title: "January 22nd, 2020 Livestream Q&A: Will consumables ever grow back?"
date: "2020-01-22"
layout: transcript
topics:
    - "environment/plants"
---
# [January 22nd, 2020 Livestream](../2020-01-22.md)
## Q&A: Will consumables ever grow back?
https://www.youtube.com/watch?v=hbm5XfpQ1O0

### Topics
* [Environment > Plants](../topics/environment/plants.md)

### Transcript

> um another one will consumables ever
>
> grow back
>
> um i don't mean
>
> no i mean i really hope so right like
>
> like some folks
>
> would be cool genuinely run out yeah
>
> there's this bug right now where it
>
> looks like they grow back
>
> um that's a bug right yeah debated
>
> there's this issue where uh especially
>
> on in multiplayer where
>
> clients will see like a bear bush and
>
> there's like berries on it and they run
>
> up and they
>
> they press like e to pick it up and then
>
> it looks like they pick it up but
>
> nothing's added to the inventory
>
> the the what's actually happened is that
>
> on server
>
> it's already picked up but it hasn't
>
> like replicated to client
>
> and updated so you don't you don't have
>
> the actual state of the bush
>
> so when you pick it up you the server
>
> notif like realizes that oh [ __ ]
>
> the client doesn't have the latest
>
> version quick hide it quick hide it
>
> and then it updates it and then you get
>
> realized oh it's just empty and you
>
> can't add anything to inventory because
>
> like there's nothing
>
> on that bush um so it's annoying and uh
>
> unfortunately that's a really big
>
> [ __ ] thing to fix
>
> it's like been on our list for literally
>
> a year to fix like because it's it's
>
> part of a big
>
> refactor that we need to do with the
>
> whole foliage system because right now
>
> the the two biggest things when it comes
>
> to networking
>
> are all the conveyor belts which we did
>
> like a big revamp off
>
> which really significantly reduced
>
> network traffic the next one is the
>
> freaking foliage system
>
> that like updates the state of all the
>
> foliage in the world
>
> uh we've had to do like a lot of custom
>
> code
>
> in unreal engine to be able to pick up
>
> foliage uh
>
> around the map because like foliage in
>
> the world is like
>
> it's batched in unreal engine so that
>
> like oh if you place like 5 000 bushes
>
> of this type
>
> it's all bashed into one draw call to
>
> some extent it's like
>
> it's more complex than that it's like uh
>
> it's batched in clusters and stuff like
>
> that very important blah blah blah
>
> but like it they have this system to set
>
> up like
>
> it's set up so that it's fast rendering
>
> but we're like but what if we want to
>
> remove
>
> one bush like that does not fly with
>
> that's just like well wait
>
> so we had to like make a very special
>
> system for that and unfortunately
>
> when we're syncing that like state to
>
> client
>
> um we send a lot of like redundant data
>
> and like data that like there's no good
>
> way to like be like
>
> is is this the same bush on service
>
> client because it's like
>
> it it's kind of random which index that
>
> bush will have
>
> yeah so we have a system that we're
>
> like going to set up that indexes
>
> indus stuff much better so that we don't
>
> need to do that and that will
>
> solve those issues unfortunately that's
>
> like one of the biggest
>
> refactorings it's so that's like that's
>
> the thing with like game dev where it's
>
> like
>
> just make a thing grow back and we're
>
> like well
>
> you know what wait we'll just we'll just
>
> put trains in the game
>
> that's easier yeah it's probably not
>
> easier but like
>
> you'd be surprised at how difficult the
>
> smallest things are some small things
>
> are freaking impossible to make and like
>
> some big things are easy so
>
> yeah really it's so annoying it's pretty
>
> and it's not like
>
> if you're a game dev you'd get it's like
>
> no game devs have no idea either yeah
>
> it's like should be fine and then you
>
> know two months later the amount of
>
> times like other game developers
>
> think they know how some systems we
>
> don't work
>
> like like we make assumptions all the
>
> time we see other games
>
> it's like oh what's it like or maybe
>
> because it's so hard to know yeah like
>
> you know even as a game developer it's
>
> really hard to know
