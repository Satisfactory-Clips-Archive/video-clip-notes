---
title: "July 8th, 2020"
date: "2020-07-08"
layout: transcript
topics: 
    - "mods"
---
# [July 8th, 2020 *Unofficial* Community Mods Showcase](../2020-07-08.md)
## Snutt Talk: How unofficial mods work (Part 1)
https://youtube.com/embed/1dUNmBBbExs?autoplay=1&start=158&end=645
### Topics
* [Mods](../topics/mods.md)

### Transcript

> this is a two-parter
> of this whole thing right because i
> don't just want to like show up like
> you're a
> bunch of cool mods without like
> acknowledging just how much
> [ __ ] work that went into uh uh
> like getting mods working whatsoever
> how much work work has gone into like
> supporting mods in general but also like
> setting up like this whole [ __ ]
> ecosystem
> of like both wrapping
> around like how you access mods if
> you're developing mods
> yourself and also like making sure that
> people can get mods
> it is an easy way so there's there's a
> lot to it so i'm just going to start
> by showing off the mod mod manager
> i'm going to i'm going to mix these up
> 50 billion times
> so essentially how do you get mods right
> that's that's probably the first
> question to answer
> um and you go to this website
> called fixing.app uh so from here this
> has been where they've been distributing
> mods
> from the get-go kind of like since we've
> had mods from the guinea
> and yeah this is where you get the mod
> manager which is
> [Music]
> really nice it's a really nice way to
> get mods you don't even need to like go
> to the website once you have the mod
> manager uh to like download and load
> mods and whatever
> and you don't even need to like [ __ ]
> like you need to install them but you
> don't actually
> uh need to because everything is managed
> in the mod manager uh
> so it's really neat so like you download
> the mod manager and then like you can
> browse
> the mods and be like yeah i want to get
> all the mods and i can look at like oh
> this looks cool
> apparently uh 16k
> where was it 16k
> um on the modding community there's
> 16k members i don't think that's on the
> website or on the discord so but anyway
> 16 000 people
> noise yes yes um why people laughing
> did i miss something because i recruited
> uh i i realized i didn't set up the
> sound so i didn't actually but
> yeah so so so
> so you can open up the mod mag and be
> like here's here's a cool mod uh passive
> oh wait oh my gosh switchback
> here's a cool mod like passive mode and
> and then it opens up like this extra
> branch and it shows like some like
> here's what the mod is about or like you
> can go here and be like
> here's the huge storage thingamajig
> really cool
> and stuff like that um so so even with
> the mod manager you can just browse and
> like check for mods itself
> uh it's really dope and you can like
> search like i want i want
> uh faces only fans
> jace oh there's not a jace mod too bad
> bummer
> um so yeah really cool and
> the thing about this as well is like
> there's there's there's
> kind of like a few more systems behind
> the scenes as well i've made i've made a
> diagram
> check this [ __ ] out let's see if i can
> find it
> boop um
> such a nerd dude i know right this is
> high school
> this isn't powerpoint this is a
> satisfactory
> all right so so the way it works right
> is that uh
> for to be able to like load mods and
> wait let me just hold up
> i'm i'm deviating from my own notes
> there's something in
> in the behind the scenes it's called the
> satisfactory mod
> loader which is like the system that
> like loads mods into the game itself
> um and that's also like
> the version like that keeps track of
> like being able to like access stuff
> in the game through the mod uh
> because for the longest time like it was
> kind of like closed off
> and that's that's what kind of like
> happens when we don't have official mod
> support yet
> is that you can't like access stuff in
> the game yet
> uh but because they made this [ __ ]
> thing
> uh and i'm trying to find the
> documentation for
> here we go right so so
> like there's a bunch of stuff that you
> need to like set up
> in order to like act to be able to make
> a mod right
> and and i just want to quickly run
> through that because just to show how
> much work
> there is behind the scenes for this
> right uh so first of all there's
> something called the mod bootstrapper
> which is like the thing that they
> they use to like access
> functions in the game to be able to like
> access unreal engine
> specific things um or you know be able
> to like
> access the r are the code that we've
> written so they can access like loading
> uh the same functions that we do
> and that's the bootstrapper and that's
> kind of like in
> behind the scenes running and then you
> have the mod loader which takes the
> like uses the bootstrapper to like
> access the stuff
> and and it handles like unpacks and
> unpacks the mods etc
> and then if you want to make your own
> mod you have to like
> download uh both the version of v-wise
> that we're using the audio engine
> you have to download like a special
> branch of unreal ending
> that they the modders have created that
> you can download on epic's
> github page um you need
> like your ide and blah blah like there's
> just so much work that goes on
> uh that's been set up just so that you
> can make mods and this is
> essentially the different like the
> different components to it right
> so you have like your different mods are
> loaded into sml
> which is then loaded into the
> bootstrapper that injects into the game
> um and then you have the satisfactory
> mod manager
> that handles all this behind the scenes
> and that also downloads
> and uh and handles it from the
> satisfactory
> mod repository this is the fixit app
> website
> a lot of stuff um
> and it blows our minds that
> that somebody wanted to set this up
> first of all uh but also like how far
> people have gotten so far it's gotten
> like so nice to use kind of thing it's
> really good
> yeah and it's it's really conv yeah that
> as well like it's so convenient to use
> like
> it you don't even need to like do
> do the classical thing of like yeah i'm
> going to download this mod and like
> place it in the folder like no you don't
> do that
> so so i'm going to show that later in
> the stream because i want to make sure
> that uh
> i don't like load in a mod that will
> crash the because i have a lot of
> mods loaded in right now and uh some
> mods don't jive with other mods for
> instance and i don't know
> which ones do um so yeah essentially you
> you pick and choose your mods you like
> find this model i want to try this out
> and uh you download it by clicking on it
> and then
> when you feel like i got everything you
> press launch game
> and uh it boots up the game it loads in
> the mods
> and you just play and the mods are in
> the game
> and that's pretty much it so simple
> yeah it just works it just works
> it is kind of to me it's kind of magic
> one other thing that i think is really
> cool that we tested
> that i didn't know this had but some
> mods also support multiplayer
> um and if you try to connect to a game
> that's running uh a modded version
> you'll get like a pop-up in the other
> one saying like oh this player is using
> a modded version and you can't connect
> to them
> even though you haven't like installed
> anything
> uh i that's magic
> i don't know if we helped out with that
> or something or if that's we'll just say
> yeah
> yeah okay i'll just better call out
> black screen mod
> yeah but i was so surprised when i saw
> that
> so here we go booting up the game bam
> and then you have like here
> it says like bootstrapper uh and then
> you have 19 mods loaded
> and you can see the mods that you've
> loaded in um
> and then you just go man you're just