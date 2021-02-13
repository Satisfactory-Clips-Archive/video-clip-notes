---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 2)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine"
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 2)
https://www.youtube.com/watch?v=cZgVZMk4zvM

### Topics
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> yeah so i wanted to show one other thing
>
> here that's of
>
> great importance is the ush file
>
> which is funny swedish that'd be the
>
> clothing of like
>
> gross uh so this is the
>
> shader header which is going to lay out
>
> our
>
> vertex factory which
>
> is essentially telling the gpu
>
> what and where in all the vertex
>
> properties we need to actually render
>
> the mesh
>
> and this is another file that has
>
> is heavily modified to support our code
>
> um the local vertex factory this is uh
>
> the primary one
>
> used for most mesh types but there's
>
> these custom macros
>
> and the syntax highlighting here sucks
>
> because this is not
>
> a cpp or c file i have uh set it to use
>
> hlsl just so that some of the float4s
>
> and
>
> macros kinda highlight um
>
> one trick i could do is like if i was to
>
> add a if define here i could define
>
> spline instancing so that it would act
>
> like these macros
>
> would they would show up better
>
> essentially but i'm not going to do that
>
> because i
>
> uh have done that before and then i
>
> forgot to remove it and
>
> i was wondering why everything was
>
> breaking and that was foolish
>
> um i'm a fool a damned fool
>
> so one major change that they've done
>
> here is they've collapsed
>
> all their spline data
>
> into one nicely compacted uh array
>
> of float fours and you can see them like
>
> putting different properties
>
> into the so the w component is getting
>
> the spline roll
>
> and that's just a scalar and then this
>
> position is a vector so that we just use
>
> these properties um
>
> quite different how they used to do it
>
> yes so this is pretty much
>
> wrapped this exact thing almost if i
>
> remember correctly
>
> like we've done our own version of this
>
> i wonder if i still like all these
>
> defines
>
> yeah exactly so yeah we had we had done
>
> them
>
> before it was below and separate and now
>
> and that was an optimization because we
>
> didn't actually necessarily need
>
> everything
>
> that they were passing in like this
>
> smooth interp roll scale we're not using
>
> um but now that they've packed it down
>
> my
>
> thinking our thinking actually is that
>
> we're going to try to use
>
> their struct here their layout instead
>
> of using our custom floats
>
> as it'll be easier to upgrade in the
>
> future and
>
> um we can minimize the duplication of
>
> code
>
> it just works it just works so we've
>
> already merged so this file is this
>
> isn't like i'm not doing the full
>
> upgrade
>
> so anywhere you see use line instancing
>
> that's a macro that we've defined
>
> and i'll show you where
>
> so in the what's
>
> it uh if i
>
> yeah so when you're declaring a vertex
>
> factory
>
> there's this wonderful function called
>
> modified compilation environment
>
> which it will call and you can pass in
>
> specific defines to use
>
> and this is ours which we have to have
>
> to use with the uh when generating the
>
> shader
>
> so if we didn't have this uh set defined
>
> in our cpp here
>
> the previous where'd it go uh
>
> that's got to be a cliche right
>
> everybody who streams trying to do this
>
> stuff where'd it go
>
> where'd it go no i think that's just you
>
> that's just me
>
> thank you okay i thought that was your
>
> cat in the background that's your coat
>
> hanger
>
> yeah let's go ahead and i don't know if
>
> you can see the coffee stained hoodie on
>
> there i legit
>
> thought that was your cat sitting like
>
> on something
>
> it's it likes to perch high yeah i'm
>
> hoping my cats don't disturb me too much
>
> or
>
> or maybe i do because they're adorable
>
> um
>
> now where was i snoot oh yeah
>
> just that's where the defined that's
>
> where the defines being passed in from
>
> the cpp code
>
> and so that's something we always have
>
> to change just to make sure it's using
>
> this
>
> but now on to some actual development
>
> i think perhaps
>
> as uh going through all these different
>
> uh structs and
>
> classes would be way outside the scope
>
> of what
>
> this could ever potentially be um and i
>
> don't even have the full
>
> understanding of this system so
>
> here we've commented out spf mandatory
>
> and then with a funny comment this
>
> should not be optional
>
> so right now it compiles and works
>
> because we've set this to optional
>
> and the reason the mesh isn't showing up
>
> is because it's
>
> these parameters just don't exist and we
>
> need them
>
> all of these to actually get the correct
>
> instance locations and render it
>
> properly
>
> so the vertices are essentially just not
>
> non-existent
>
> because these parameters are not working
>
> so they should be this mandatory
>
> so i'm going to switch them
>
> now as some of you may guess
>
> if i so yeah this is where i just make
>
> it that makes it
>
> not read only um
>
> if i was to compile and run this
>
> i would get a shader error crash while
>
> booting
>
> um and that's something i'm aware of
>
> so i don't want to do that because it
>
> would just take long to show you how
>
> much it fails
>
> so now that they're mandatory we need to
>
> get these parameters
>
> in there
