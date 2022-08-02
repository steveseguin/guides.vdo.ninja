---
layout:       post
title:        "Two person chat"
date:         2020-12-16 10:00:00 +0000
author:       "Steve Seguin"
categories:   basic
tags:         tag1 tag2
permalink:    2personchat
order:        4

# POSTS LIST
class:       "style3"                         # config bg-color to post list card (1..6)
list-image:  "/assets/images/pic04.jpg"       # config image to post list card (1..6)
description: >                                # config description to post list card
  Get your camera inside VDO.ninja quickly

# POST HEADER
header-image: "/assets/images/pic13.jpg"      # config image to post header
alt-image:    "image description test post a" # config image description to alt att.
---

While you can achieve a multi-person chat with a group room, and that's the recommended way, you can also do it without using a room.

For example, `https://vdo.ninja/?view=xxxxxxx&push=yyyyyy` will let you publish your video and video a remote video at the same time.

You'll notice here that we have the link both PUSHing and VIEWing at the same time. This allows us to view a remote video and publish a video to others, using the same website tab.  This has the advantage over using two-browser tabs (one for pushing and one for viewing) as echo-cancellation will work with this approach, while with two-tabs it would not. It also is compatible with mobile-devices, where two-tabs isn't likely feasible.

The downside of this approach is that you'll need to create a custom link for every person. In this case, 

`https://vdo.ninja/?view=xxxxxxx&push=yyyyyy`
and
`https://vdo.ninja/?view=yyyyyy&push=xxxxxxx`

To ingest a remote guest's video into OBS or other studio software, it is common to then use a dedicated view-link for each guest. For example:

To view just one video: `https://vdo.ninja/?view=yyyyyy`
Or to view both videos side-by-side as a single mix: `https://vdo.ninja/?view=yyyyyy,xxxxxxx`

In this setup, a guest would be pushing two video streams; one stream to the host, and one stream to OBS for capture. This creates some load on the remote guest, and while most modern computers can handle this, you may wish to optimize the bitrates to reduce this load.

So, `https://vdo.ninja/?view=xxxxxxx&push=yyyyyy&bitrate=500` would limit the bitrate to 500-kbps, while the link that is added to OBS can be set to something higher.

For example `https://vdo.ninja/?view=xxxxxxx&bitrate=4000` would have the OBS view of the remote video be captured at 4000-kbps; higher than the default 2500-kbps.

There's numerous other ways to optimize how you use view and push links of course, but when using a group room instead, most of the optimizations are already handled for you.

For example,
`https://vdo.ninja/?room=zzzzzzz`

or for something even cleaner,
`https://vdo.ninja/zzzzzzz`


For more advanced users looking to improve audio quality, consider going deeper with understanding the `&proaudio` URL parameter, which can enable high quality 256-kbps audio.  There are endless additional tweaks and options, which you can references at https://docs.vdo.ninja
