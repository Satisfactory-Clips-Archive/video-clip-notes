---
title: "October 9th, 2020 Livestream Dylan Talk: Instanced Splines (Part 6)"
date: "2020-10-09"
layout: transcript
topics:
    - "technology/unreal-engine/custom-component-instanced-spline-mesh"
---
# [October 9th, 2020 Livestream](../2020-10-09.md)
## Dylan Talk: Instanced Splines (Part 6)
https://www.youtube.com/watch?v=tvqEYd2LI1A

### Topics
* [Technology > Unreal Engine > Custom Component: Instanced Spline Mesh](../topics/technology/unreal-engine/custom-component-instanced-spline-mesh.md)

### Transcript

> okay so i found what i was looking for
>
> actually
>
> let's continue on so this is in their
>
> spline mesh component
>
> um we can see where they how they're
>
> setting up their
>
> data bindings and i'm going to actually
>
> copy that because i want that verbatim
>
> so we get element shader bindings
>
> which we have declared externally right
>
> yep so in this we had our
>
> old setup of shader bindings which is at
>
> the bottom here
>
> and this was because we were binding
>
> specifically to those parameters
>
> um but now we're trying to match theirs
>
> more one-to-one as they've
>
> optimized it and uh packed them in
>
> nicely
>
> so it doesn't feel like a waste to do it
>
> this way
>
> um so i'm going to actually just
>
> comment out ours that this is like our
>
> old one
>
> and slam a dam in there is there
>
> this is lava david slam a damn name and
>
> i should
>
> i i'm gonna go back there we always mark
>
> up uh when we change
>
> these files with our cs tags css and
>
> this makes
>
> merging way way easier in the future but
>
> um so we can see if something's
>
> intentional or if they change something
>
> or if we
>
> intentionally changed it leave a comment
>
> but for i'll do that
>
> that's not fun so i'm going to not worry
>
> about that at the moment
>
> now i'm just taking a look at make sure
>
> there's no
>
> conflicts there
>
> looks good so now we've changed the
>
> instance binding parameter map to just
>
> bind
>
> i didn't finish that that's right it
>
> does nothing we bind text
>
> null text i want to see their bindings
>
> show me your bindings
>
> such as two
>
> this is the in it
>
> where is there i'm just being done
>
> okay it's gonna be in the head
>
> i was in our file i see i am being done
>
> take a look
>
