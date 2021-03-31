---
title: "March 30th, 2021 Livestream Q&A: What's the Object Limit?"
date: "2021-03-30"
layout: transcript
topics:
    - "technology/unreal-engine/object-limit"
---
# [March 30th, 2021 Livestream](../2021-03-30.md)
## Q&A: What's the Object Limit?
https://www.youtube.com/watch?v=KjV7JMFQ3Is
<details>
<summary>This question may have been asked previously at least 9 other times, as recently as October 2020 and as early as August 2020.</summary>

* October 9th, 2020 Livestream Q&A: What is the limit? [https://www.youtube.com/watch?v=Njv_PJT3B2g](https://www.youtube.com/watch?v=Njv_PJT3B2g)
* October 6th, 2020 Livestream Q&A: What is the object limit and why is it that number? [https://www.youtube.com/watch?v=VpCuu0aYFw0](https://www.youtube.com/watch?v=VpCuu0aYFw0)
* September 1st, 2020 Livestream Q&A: Have you thought about implementing a progress bar for how close to the Build Limit we are? [https://www.youtube.com/watch?v=RyE_hc4huhA](https://www.youtube.com/watch?v=RyE_hc4huhA)
* August 18th, 2020 Livestream Build Limit (Part 1): [https://clips.twitch.tv/SplendidAffluentVampireNotLikeThis](https://clips.twitch.tv/SplendidAffluentVampireNotLikeThis)
* August 18th, 2020 Livestream Build Limit (Part 2): [https://clips.twitch.tv/UnusualExquisiteKuduDendiFace](https://clips.twitch.tv/UnusualExquisiteKuduDendiFace)
* August 18th, 2020 Livestream Build Limit (Part 3): [https://clips.twitch.tv/SullenColdbloodedDiscEagleEye](https://clips.twitch.tv/SullenColdbloodedDiscEagleEye)
* August 18th, 2020 Livestream Build Limit (Part 4): [https://clips.twitch.tv/BlitheEnergeticEelPRChase](https://clips.twitch.tv/BlitheEnergeticEelPRChase)
* August 18th, 2020 Livestream Build Limit (Part 5): [https://clips.twitch.tv/GiantGeniusGooseCclamChamp](https://clips.twitch.tv/GiantGeniusGooseCclamChamp)
* August 18th, 2020 Livestream Build Limit (Part 6): [https://clips.twitch.tv/BoxySmallAsparagusSmoocherZ](https://clips.twitch.tv/BoxySmallAsparagusSmoocherZ)
</details>


### Topics
* [Technology > Unreal Engine > Object Limit](../topics/technology/unreal-engine/object-limit.md)

### Transcript

> what's the object so
>
> i again i i say this every time and i
>
> know i'm not going to be able to
>
> to um educate enough people so that this
>
> this will change but it's it's not an
>
> object limit you guys it's a memory
>
> limit
>
> it's a memory limit of how many objects
>
> the engine can keep track of at a time
>
> and it's not an
>
> object in terms of like physical objects
>
> in the world
>
> it's memory allocated memory
>
> like spaces and those are referred to as
>
> memory objects
>
> because of programming paradigms
>
> it's it's it's memory objects not game
>
> objects
>
> a game object can have many memory
>
> objects and
>
> a game object can have n number of
>
> memory objects so it's not one to one
>
> either
>
> so but the limit is like something two
>
> million
>
> u objects that's why i always like
>
> i want to point out that it's you object
>
> not object
>
> limits um and i've explained this a
>
> billion times and it's it's it really
>
> isn't
>
> if you're not a programmer this doesn't
>
> make sense
>
> because of the way we it's a linguistic
>
> thing the way we describe it
>
> um the fact that we we need programming
>
> we kind of need to like create physical
>
> things to talk about we need to
>
> anthropomorphize some things
>
> because it makes makes it easier to talk
>
> about things and that's kind of like
>
> kind of up when we talk about this
>
> thing
>
> yeah i'm a programmer it makes a perfect
>
> sense yeah but the people that aren't
>
> programmers it doesn't make sense so
>
> people think oh object limit that must
>
> be game objects
>
> but that's not the case so that's why
>
> it's kind of confusing
>
> um because we can't change the the u
>
> object limit
>
> we can't optimize for it so potentially
>
> you could if you build like
>
> x amount of objects and it crashes the
>
> game and hit that limit
>
> we could optimize it so that you could
>
> potentially load that game again without
>
> changing the limit
>
> yeah it's an engine limit and another
>
> thing to point out as well
>
> it's an engine limit but you can
>
> technically increase it if you go to the
>
> config files but we don't recommend that
>
> because we don't know what happens if
>
> you do
>
> you can get very weird memory issues
>
> uh when you play the game and it can be
>
> as bad as it corrupts your save file and
>
> it in fact
>
> has happened for people so we know it
>
> can happen um
>
> that's why we don't recommend it if you
>
> do want if you have built
>
> a base that's so big that you hit that
>
> limit then what you can do is
>
> back up your save file then go into the
>
> config files and change it
>
> but be aware that that may cause issues
>
> down the line
>
> and if we do optimize the game
>
> further down the line where the limit is
>
> better
>
> the config files will not get overridden
>
> so your manual change of the config
>
> files will still persist
>
> and you could potentially be playing a
>
> version of the game where we've fixed
>
> most of those issues
>
> and you get a corrupt save file and that
>
> sucks
>
> so that's why we're really clear about
>
> the fact that
>
> there is a way for you but we don't
>
> recommend it because it could cause
>
> issues
>
> uh so you're you're 100 on your own if
>
> you if you do that
>
> but we we are not stopping you you're
>
> free to do whatever you want there
>
> but just know that this is a complicated
>
> problem
>
> so re like really read up on it um
>
> before doing anything and read up on it
>
> means
>
> listen to us don't listen to community
>
> community because this is like
>
> super construed what people think the
>
> problem is and what the solution is and
>
> the idea
>
> of how it works like there are
>
> i think we've put out some video about
>
> it somewhere around where
>
> you can quote that or maybe we should
>
> make a video about it or something i
>
> don't know it's kind of
>
> scary also because we don't want you
>
> guys to like build
>
> in a certain way that like is optimized
>
> because that's not
>
> fun it's uh it's on us to make the game
>
> fit your play needs you know
>
> it shouldn't be the other way around
>
> maybe it's it's the other way around for
>
> now because we're still optimizing the
>
> game and the game isn't done
>
> and if you want to like keep playing
>
> maybe you need to
>
> but it shouldn't be on you guys it
>
> should be on us to fix those kind of
>
> things
>
> all right i
>
> always get so flushed when i
>
> talk about this but it's just like
>
> it's it's a it's a it's a little bit
>
> frustrating for me because
>
> it's so misconstrued in community people
>
> talk about it in one way but it doesn't
>
> work that way
>
> um and it's just really hard to get that
>
> information out
>
> because it's a complicated subject and
>
> there's no like easy
>
> easy way to explain it i think
>
> um so i can only keep trying
>
> but i'm also okay with it the fact that
>
> like this is the way
>
> you get as a community manager like you
>
> never reach everyone there's always
>
> going to be misconceptions about
>
> everything
>
> so uh but yeah i'll i'll keep explaining
>
> it as many times
>
> as i as i need to uh for as long as that
>
> problem exists i don't mind it
>
> um we just gotta keep doing our best you
>
> know
