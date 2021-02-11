---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 1)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 1)
https://www.youtube.com/watch?v=c6Qy5jzXmqM

### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> but the reason for this is we use a
> 
> custom component called uh
> 
> instant spline which isn't native to
> 
> unreal engine
> 
> they don't have an implementation of it
> 
> um they do
> 
> have splines so you can make like and a
> 
> spline is basically a
> 
> grouping of curves that create you know
> 
> nice smooth lines essentially that's a
> 
> very poor way of explaining that
> 
> but you can with a mesh component supply
> 
> mesh component you can put a bunch of
> 
> mesh
> 
> meshes along the spline and creates a
> 
> nice curved from just a single static
> 
> mesh
> 
> so like if i was to open up our it also
> 
> bends the mesh
> 
> so yeah it lines properly yeah exactly
> 
> it lines up all the vertices
> 
> again so like this is what our conveyor
> 
> mesh looks like
> 
> and that's it and that's it and then it
> 
> gets strung along the spline
> 
> and bent and curved and lines up and
> 
> looks nice
> 
> this is the same thing with pipes
> 
> actually so if i was to build uh pipes
> 
> now
> 
> which i will do so you can see the the
> 
> extent of this
> 
> breaking i don't think this this issue
> 
> is funny so
> 
> oh so many things and and you don't know
> 
> that you're going to get these issues
> 
> when you
> 
> upgrade either i mean this one we kind
> 
> of knew
> 
> ah damn it you got to turn on the
> 
> no cost
> 
> because they don't have this natively in
> 
> the engine
> 
> we had to create our own implementation
> 
> which i did not create
> 
> so you can see yeah that's the indicator
> 
> but where's the
> 
> where's the pipe okay so they're
> 
> essentially used in the same space they
> 
> use
> 
> yeah instant static mesh component and
> 
> how we do that is we take
> 
> their existing component
> 
> which is a instant static mesh
> 
> and kind of co-opt it into
> 
> an instant spline mesh so every time we
> 
> upgrade the engine this is typically the
> 
> most painful part
> 
> where we have to take all of their
> 
> changes to the static mesh code instant
> 
> static mesh code and convert it into our
> 
> custom
> 
> spline mesh instant spline mesh code
> 
> and this so this is a diff of the two
> 
> files
> 
> we have on the left here is their
> 
> version of the static mesh
> 
> and then r 423 so this is our 423
> 
> upgrade
> 
> of our spline mesh and these are the
> 
> cpps
> 
> so you can see how different they are
> 
> and we've actually already gone through
> 
> this and merged
> 
> all of these
> 
> and ended up with this version here
> 
> this is actual code environment and this
> 
> is what you guys are seeing just now
> 
> it doesn't work right
> 
> it works it doesn't crash this was
> 
> crashing for a long time too and the
> 
> the last two days before this was fixing
> 
> some crash books pertaining to
> 
> these as well but now i'm going to
> 
> fix it dm yeah
> 
> so the key key parts of this are the
> 
> instant spline mesh
> 
> and our cut we uh prepend and fg
> 
> to all our classes so that's
> 
> factory game spline mesh
> 
> so initially when we're going through
> 
> this we saw that we even
> 
> like is this gonna work we tried to make
> 
> it work
> 
> but we have some solid to do's on here
> 
> um and this will be this is a lot of
> 
> code
> 
> and i there's zero percent chance i will
> 
> get through all of it
> 
> like explaining all of it but i'll try
> 
> to do my best and if anyone has any
> 
> questions
> 
> please uh please chime in as new we'll
> 
> probably
> 
> relay them to me i will feed him yeah
> 
> so also i i also noticed right just now
> 
> that i had a typo in the title
> 
> of the stream i've i've fixed that chat
> 
> all right calm down
> 
> this is why we don't have nice things
> 
> you're you're a poor grammar
> 
> right poor poor grammar
> 
> i have poor grammar yes yes yeah
> 
> so they have made a lot of changes
> 
> in the last couple of engine versions to
> 
> the way their rendering pipeline works
> 
> all for the better in the long run i
> 
> think but all for the worse when we try
> 
> to upgrade
> 
> our custom component the spline mesh
> 
> here
> 
> because the changes are significant as i
> 
> just showed you from the merge
> 
> differences there
> 
> that there's a lot of things that have
> 
> changed and
> 
> we have to figure out what we need and
> 
> what we don't need
> 
> essentially because we actually in a lot
> 
> of cases
> 
> we'll just uh comment things out
> 
> completely
> 
> like this this if zero we keep these
> 
> here
> 
> to make merging in the future easier so
> 
> we can see what was intended
> 
> from their files so it might like look
> 
> ugly and like lazy programming but this
> 
> is actually intentional
> 
> so that when we take their new version
> 
> the diff will line up
> 
> correctly
> 
