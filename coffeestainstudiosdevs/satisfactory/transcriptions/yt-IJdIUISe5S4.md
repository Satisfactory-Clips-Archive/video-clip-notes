---
title: "May 19th, 2020 Livestream Q&A: Why can't you just add lights to the game?"
date: "2020-05-19"
layout: transcript
topics:
    - "features/planned-features/lights"
    - "technology/unreal-engine"
---
# [May 19th, 2020 Livestream](../2020-05-19.md)
## Q&A: Why can't you just add lights to the game?
https://www.youtube.com/watch?v=IJdIUISe5S4
This question was possibly duplicated with a more recent answer: [January 26th, 2021 Livestream Q&A: Lights & Lampposts please?](./yt-xXbrwFqiS5g.md) https://www.youtube.com/watch?v=xXbrwFqiS5g


### Topics
* [Features > Planned Features > Lights](../topics/features/planned-features/lights.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> yeah so while we're on that subject why
>
> not talk about lights a bit
>
> uh a lot of people have been asking like
>
> why
>
> why we can't just add lights to the game
>
> and we just said like it's it's
>
> difficult but maybe you can go more in
>
> depth as to like what
>
> okay so so first of all you talked a
>
> little bit about
>
> uh the optimization like but you know
>
> like the performance budget
>
> uh what you call it yeah uh and like
>
> there is
>
> it's another thing to that that is worth
>
> keeping in mind is that
>
> we don't know exactly where the game
>
> will end up
>
> so exactly what we are required in the
>
> end to render
>
> and what that will require uh
>
> in other respects we don't really know
>
> like for example
>
> right now we can build huge factories we
>
> actually run into the
>
> limit of the energy and how many objects
>
> we can have in the scene yeah
>
> and that takes time to process and what
>
> will happen with that what will happen
>
> what kind of new structures will we have
>
> what kind of
>
> i don't know it is like there are so
>
> many things that can change the final
>
> work what we what we really need for
>
> story things we need something for it's
>
> it's hard to say so we need to always
>
> keep a little user budget so we don't
>
> have to step
>
> down things later because of new
>
> requirements that
>
> actually needed for like a core feature
>
> in the game
>
> uh but then with that in mind uh
>
> lighting is very hard because it's so
>
> unpredictable and it's it's not logical
>
> for most people
>
> to understand why it's demanding so if
>
> it's suddenly starts
>
> tanking your frame rate you might not
>
> know
>
> why by yourself
>
> and we kind of have a responsibility to
>
> make that kind of understandable like
>
> right now you can't take tank the frame
>
> rate by just building a lot of
>
> structures that are expensive to render
>
> you can you can do that because
>
> the start of a game and the end game
>
> kind of base
>
> is a huge difference in performance um
>
> it's inevitable
>
> you can't get around that um so we
>
> already have
>
> that issue but it's more predictable
>
> with
>
> meshes it's less predictable with lights
>
> because
>
> the cost of lights is not um
>
> how many you have or how
>
> big they are or something like that it's
>
> it's a combination it's
>
> how many pixels on the frame is
>
> processed by light and
>
> for a model one model covers another
>
> model a light doesn't cover another
>
> light
>
> it means that you can see essentially
>
> infinite number of lights on the screen
>
> at the same time
>
> and that's that can become an issue so
>
> all these kind of things is things that
>
> we can solve and we can work around
>
> like we can turn off we can group lights
>
> on the distance like
>
> only have one of them on and increase
>
> the size and like
>
> do all kind of things that we can do to
>
> try to keep lights on and like
>
> a lot of them at the same time and i
>
> would love to
>
> it's just that it takes a lot of time in
>
> consideration to do it good
>
> yeah and
>
> it's like we have a lot of other things
>
> to do so it's always private
>
> prioritization can we do lights now can
>
> we do this now
>
> it's yeah yeah it's a it's a really
>
> interesting kind of optimization problem
>
> i think
>
> uh yeah yeah but it's it's a big
>
> thing and and we don't have enough big
>
> things in the game already
>
> to solve um like in both in terms of
>
> like networking and
>
> like all the other things in the game um
>
> so yeah
>
> yeah and and like some people's
>
> computers might handle them just fine
>
> until they reach down the game and they
>
> have a really expensive base and it's
>
> yeah it's it's i understand the
>
> frustration from some people like they
>
> have a
>
> really strong piece they have good frame
>
> rate and yes one lights uh
>
> but that's not the case for every player
>
> and the
>
> yeah yeah that's that's another thing
>
> that we have to consider everybody
>
> like we can't just consider the high-end
>
> the people that have high-end pcs like
>
> we have
>
> we have a responsibility to make sure
>
> that the game kind of runs for everybody
>
> um we can work on those
>
> like more exclusive stuff for the people
>
> who actually just a few people who can
>
> use it
>
> later potentially but most of the time
>
> you
>
> want to work on the things that give the
>
> most bang for the buck for most people
>
> like it's
>
> yeah yeah so update first lights all
>
> right cool confirm all right fantastic
