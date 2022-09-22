---
title: "May 17th, 2022 Livestream Q&A: Map Marker limit as config thing?"
date: "2022-05-17"
layout: transcript
topics:
    - "features/requested-features"
    - "satisfactory-updates/released/satisfactory-update-6"
    - "technology/user-interface/markers"
    - "technology/user-interface/stamps"
---
# [May 17th, 2022 Livestream](../2022-05-17.md)
## Q&A: Map Marker limit as config thing?
https://www.youtube.com/watch?v=l-LVFsZi9_E

### Topics
* [Features > Requested Features](../topics/features/requested-features.md)
* [Satisfactory Updates > Released > Satisfactory Update 6](../topics/satisfactory-updates/released/satisfactory-update-6.md)
* [Technology > User Interface > Markers](../topics/technology/user-interface/markers.md)
* [Technology > User Interface > Stamps](../topics/technology/user-interface/stamps.md)

### Transcript

> [Music]
>
> map marker is a config thing tweakable for those who need it, maybe there's there's there's another there's like a there's a limitation in and what, it's called data type we're using for those
>
> [Music]
>
> because we're, since we're like I don't think I've put this out in the video but everything you see on the map that's going to work in multiplayer as well right so you're going to be able to see you know the other players on the map you're going to see their markers, etc etc okay, and when it comes to networking you always want to like, make sure that you're not replicating too much data so the the smaller data values you can send the better if you can send bits instead of bytes you want to do that so right now we're sending like a byte for those stamped things and the max value for a byte is 255, unsigned so yeah so so that's why,
>
> [Music]
>
> like the max value might be 255 because of that and then we have to prioritize like is it worth actually sending the extra data in the cache we'll see but there might be reasons because of that
>
> [Music]
