---
title: "May 19th, 2020 Livestream Q&A: Any work on Occlusion Culling?"
date: "2020-05-19"
layout: transcript
topics:
    - "technology/graphics"
    - "technology/unreal-engine"
---
# [May 19th, 2020 Livestream](../2020-05-19.md)
## Q&A: Any work on Occlusion Culling?
https://www.youtube.com/watch?v=SauDZG88AFI

### Topics
* [Technology > Graphics](../topics/technology/graphics.md)
* [Technology > Unreal Engine](../topics/technology/unreal-engine.md)

### Transcript

> any work on occlusion calling i don't
> 
> know if
> 
> actually occlusion calling we have it
> 
> yeah
> 
> but it's it's it's it's epic solution
> 
> for it and it's it's
> 
> uh it's good
> 
> it's really good because it will be
> 
> turned off it's it's worse than not
> 
> having it
> 
> but it's something i would like to
> 
> investigate more because we are spending
> 
> a lot of time
> 
> in the frame to actually do the calling
> 
> because we have such a dynamic
> 
> world of like a lot of buildings that
> 
> you place manually yeah
> 
> but the because for the longest time
> 
> it's been the case where like if you if
> 
> you because this is a question that
> 
> people ask a lot
> 
> it's like if you build walls around your
> 
> factory
> 
> uh it doesn't act like for the longest
> 
> time satisfactory hasn't like
> 
> occluded that inner part in the factory
> 
> so like
> 
> walls wouldn't occlude them there's two
> 
> things to this so
> 
> it actually has for a long time but
> 
> there is actually a problem when you
> 
> it can only use the last frames data
> 
> like what you saw in the last frame and
> 
> use depth information from that to call
> 
> objects in the current frame which means
> 
> that if you are standing and looking
> 
> away from this wall and then you turn in
> 
> one frame and look against the wall
> 
> you don't have any depth information
> 
> about the wall meaning you can't do
> 
> any occlusion at all so you have to draw
> 
> everything for one frame
> 
> and then after that you have the
> 
> information and then you can start
> 
> calling
> 
> and that's not ideal because it gets
> 
> stutters when you move the camera a lot
> 
> inside
> 
> a very heavy base yeah
> 
> i've been meaning to make like a video
> 
> about this for for the longest time
> 
> because
> 
> it really is like it's not super
> 
> obvious in what circumstances you
> 
> you get these issues uh and like the
> 
> best way really to to
> 
> to know that is to do the you know the
> 
> freeze rendering and like actually move
> 
> around and
> 
> look at the word like what happen
> 
> actually happens when you do certain
> 
> things
> 
> uh so maybe that video i can make that
> 
> sometimes
> 
> but do you think they're what do you
> 
> do do you think there are things we can
> 
> do to improve that as well
> 
> i hope so like there are things that i
> 
> have in mind that i
> 
> want to do and or test but it's so hard
> 
> to predict how much
> 
> it will affect only if it will actually
> 
> be worse in cases so
> 
> it's like i can't promise anything about
> 
> it and actually do
> 
> going in and rewriting calling in the
> 
> engine is
> 
> kind of deep inside the cuts of the
> 
> rendering engine
> 
> and that's a lot of work uh
> 
> that a lot of time that could be spent
> 
> on potentially other things so like
> 
> other optimizations and so on so
> 
> we'll see yeah
> 
