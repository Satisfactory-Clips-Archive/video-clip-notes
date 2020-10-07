# [September 22nd, 2020 livestream](../2020-09-22.md)
## Q&A: Are there specific parts or objects that contain a lot of objects in them ?
https://www.youtube.com/watch?v=DDHlxZV39B0
> on that route and tried it out at least
> 
> are there
> 
> other objects that um contain like a are
> 
> there specific parts or objects that
> 
> contain a lot of objects within them so
> 
> we can avoid
> 
> building a lot of these yeah maybe
> 
> it's so hard to to say exactly because i
> 
> i certainly don't know you know all the
> 
> ins and outs of
> 
> everything like how everything's
> 
> constructed like in terms of
> 
> how we've made them how the like data
> 
> structures
> 
> off the object so to speak are set up
> 
> and whatnot and contribute to the object
> 
> count
> 
> exactly because there's a lot of um like
> 
> for instance we've done a number of
> 
> optimizations for networking
> 
> where we kind of need to duplicate a lot
> 
> of stuff and then
> 
> replicate that so on the server that
> 
> means that for every building
> 
> that you interact with you'll create a
> 
> double um
> 
> so it's like that's an optimization for
> 
> network but that's also
> 
> worse when it comes to the object count
> 
> thing uh
> 
> so like there's there's so many
> 
> different cases
> 
> with that specific issue um
> 
> [Music]
> 
> and maybe we need to in the way in the
> 
> future maybe we need to
> 
> rewrite how memory management works for
> 
> like certain buildings or something just
> 
> to get that number count down
> 
> like there are a lot of different routes
> 
> we can take to improve that
> 
> and we are taking some of the routes
> 
> right now um but uh yeah
> 
> it's it's a really tricky subject to
> 
> talk about because i actually don't know
> 
> what the
> 
> like best because i know a lot of people
> 
> ask me like what's the best way to build
> 
> to not run into that issue and i
> 
> actually don't know because it's
> 
> it's so different like we we get we can
> 
> like when we collect saves we'll get
> 
> like one that's like oh this is like
> 
> rarely
> 
> there's not almost anything on the same
> 
> but yet the object count is really high
> 
> and then we have another save that has
> 
> like a [ __ ] ton of stuff on it
> 
> but the object count is really low and
> 
> it really is like
> 
> so many different scenarios that's kind
> 
> of like attributed to that object cam
> 
> so it's really hard to give advice on
> 
> that
> 
> um maybe
> 
> like maybe in the future we can have
> 
> either
> 
> like one of the programmers on that know
> 
> more about this or or
> 
> someone else uh to talk more about this
> 
> stuff if it's interesting
> 
> um so yeah but it's yeah it's really
> 
> hard
> 
> to say just don't use the garbage like i
> 
> mean that's a
> 
> legit way to go about it we would need
> 
> to rewrite
> 
> a ton of stuff uh but that's that's
> 
> legit one one way to go about it
> 
> so yeah long story short uh i don't
> 
> [ __ ] know
> 
