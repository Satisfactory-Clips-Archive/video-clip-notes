---
title: "September 25th, 2019"
date: "2019-09-25"
layout: transcript
topics: 
    - "features/save-system"
    - "features/save-system/cloud-sync"
---
# [September 25th, 2019 Minor Patch Info - Train fixes & Cloud Saves](../2019-09-25.md)
## Snut Talk: Save Files & Cloud Saves
https://youtube.com/embed/t1LfyNfuMVQ?autoplay=1&start=100&end=187
### Topics
* [Features > Save System](../topics/features/save-system.md)
* [Features > Save System > Cloud Sync](../topics/features/save-system/cloud-sync.md)

### Transcript

> files and make sure to take notes
> because this is all gonna be on the test
> so in the next patch we're introducing
> cloud safe so satisfactory on the epics
> game store
> big bro team Sweeney got us hooked up
> but in order for us to support cloud
> safe so we've had to make a few
> adjustments to our current safe
> structure of the game so let me first
> point out that as a whole the safe
> system will work pretty much the same
> way as before you can still like grab
> your safe files and save directory and
> like share them with your friends so
> throw them out the window what are you
> going to do with them the only
> difference now
> that save files will be placed in sub
> directories instead and those sub
> directors will be synced via the epic
> games launcher so essentially when
> you're playing the game and you're
> saving that save file will be placed in
> a directory that's associated with your
> epic account so immediately not all your
> safe files will be converted into this
> new safe structure and cloud synced and
> that's because up until this point we
> haven't compressed our save files and
> what that means is that the save files
> can get quite large and that's not
> optimal if you want to cloud sync them
> and in order to do that you need to load
> up your safe file and then we save it
> for it to be able to like be converted
> moved into the epic account folder and
> then it can be cloud sinks and all the
> files that haven't been associated with
> an epic account ID yet will be placed in
> a fuller called common in the same
> directory and they'll be placed there
