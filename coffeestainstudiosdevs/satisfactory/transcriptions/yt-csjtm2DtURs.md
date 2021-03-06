---
title: "October 9th, 2020 Livestream Snutt & Dylan Talk: Updating the save system"
date: "2020-10-09"
layout: transcript
topics:
    - "coffee-stainers/dylan"
    - "features/save-system"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Snutt & Dylan Talk: Updating the save system
https://www.youtube.com/watch?v=csjtm2DtURs

### Topics
* [Coffee Stainers > Dylan](../topics/coffee-stainers/dylan.md)
* [Features > Save System](../topics/features/save-system.md)

### Transcript

> jalen is working on updating this our
>
> save system which i've talked about a
>
> lot on our show oh yeah
>
> but i have no idea why we're doing that
>
> why we're doing the save system
>
> yeah or why we're redoing it or changing
>
> it yeah i know
>
> roughly but i think you're better at
>
> explaining it because you're the one
>
> that's actually doing it
>
> yeah sure sure that's good logic um
>
> uh let's see i was actually thinking
>
> about doing that for this stream instead
>
> but this felt more uh constructive
>
> because we need to get we want to get
>
> the engine
>
> up and going as fast as possible
>
> so i'm actually launching the editor now
>
> to see if it works um but it's on the
>
> other screen so you won't be able to see
>
> it unfortunately
>
> um but yeah we're changing the save
>
> system so right now everything
>
> that is saved has to be in persistent
>
> worlds
>
> or always loaded levels which means when
>
> you load the game
>
> it has to load like every destructible
>
> rock
>
> check to see if it's still there and all
>
> this stuff
>
> and it means that well for one it's bad
>
> for
>
> rendering because you have a lot of
>
> really far away calling objects
>
> it stopped us from adding features
>
> before because we didn't want to
>
> introduce more
>
> world actors that are always present
>
> which is just basically continually
>
> hurting performance
>
> so what i'm doing is i and this is
>
> actually
>
> uh done-ish
>
> but it probably won't go live for a
>
> little while for behind the scenes
>
> reasons
>
> but um essentially now we can
>
> save these actors in the streaming tiles
>
> so when you load in like when you stream
>
> in a new tile we can have the actors in
>
> there
>
> verse having them in the always loaded
>
> worlds
>
> um and there's like 10 000 like actors
>
> that just
>
> are always there with from destructible
>
> rocks to slugs
>
> what have you spore flowers and that's
>
> bad
>
> we didn't like that but it is also
>
> a pain and there's a gonna be a
>
> migration process and that's a little
>
> bit of
>
> a little problematic and we also don't
>
> want to
>
> you know ruin people's safes so
>
> i do think we're going to have to have a
>
> little pow wow with the
>
> save editor though because that's such a
>
> nice tool
>
> but it's going to i was reminded because
>
> i i also was reminded because i saw
>
> anther here
>
> who's worked a lot on the satisfactory
>
> calculator site oh nice
>
> when we changed that
>
> um yeah so i said before we were
>
> we had one root set where we would
>
> serialize uh everything down into
>
> like one archive and now we have a per
>
> level archive
>
> so each tile gets its own archive to get
>
> saved
>
> i most of the logic i think i
>
> i say this without having looked at the
>
> code for those things we'll translate
>
> and you'll just have to do some
>
> modifications to kind of redirect it
>
> but i think we'll also like we'll
>
> probably be helping out people that want
>
> to know the save archive structure and
>
> everything when the time comes
>
> this is still a ways off does that have
>
> any impact on like the save time
>
> in game um yes
>
> ish theoretically it's reduced because
>
> we're not having to save the world
>
> actors so every time a tile is streamed
>
> out
>
> it saves like it doesn't have it saves
>
> its archive
>
> it won't change the disk right time um
>
> which is actually not most the time
>
> anyway
>
> but uh in my tests it was
>
> almost identical unfortunately but that
>
> was
>
> on massive factories and we're talking
>
> like
>
> 100 to 200 000 factory objects versus
>
> the 10 000
>
> world objects that are no longer being
>
> serialized down
>
> so it was you know fairly insignificant
>
> when you're comparing those
>
> that scale so for people on smaller
>
> bases or slower computers
>
> you'll likely see an increase i can
>
> reduce i guess at reduce save time
>
> but yeah it's it's more it will
>
> get to that at some point there is yeah
>
> that was that's
>
> a separate task kind of it was while i
>
> was working on this it was
>
> i was finding places to optimize but we
>
> didn't want to make that the focus of
>
> that we want to get that working first
>
> and then right you don't want to
>
> introduce more bugs than you
>
> when you're completely overhauling such
>
> a key system like that
