---
layout:       post
title:        "Mobile phone camera into webcam"
date:         2020-12-17 23:31:00 +0000
author:       "Steve Seguin"
categories:   basic
tags:         basics
permalink:    phone-camera-to-webcam
order:        6

# POSTS LIST
class:       "style1"                         # config bg-color to post list card (1..6)
list-image:  "/assets/images/pic07.jpg"       # config image to post list card (1..6)
description: >                                # site meta description
  Learn how to leverage VDO.Ninja to bring your phone's camera as a desktop webcam.
list_description: >
  High quality webcam with just your phone.


# POST HEADER
#header-image: "/assets/images/4kComparison.png"      # config image to post header
alt-image:    ""                                  # config image description to alt att.
---


This set of instructions will work for Windows, Mac[^1] and Linux[^2].

## How to use

1. Bring your VDO.Ninja 'view' link into OBS. Drag and drop the link into a scene, and resize it to fit. Make sure OBS has audio control
2. Take your scene and make it the 'program' output in OBS if in studio mode.
3. On the main UI press "Start Virtual Camera"
4. Open your 3rd party program and choose "OBS-Camera" as a Video input


## Use Cases

OBS VirtualCam is fully compatible with VDO.Ninja and is useful for connecting MULTIPLE different OBS mixers together remotely, so you can take turn producing a show. You can also use it to turn your smartphone into webcam. You can also share your "live show" with a small group of friends, perhaps those who are also in the show with you, so everyone has a real-time view of the show that is going on.

## Notes

Sometimes you may need to stop/restart the VirtualCam if it starts crashing your computer. If you see nothing but "GREY", then you need to start it before using it. See "How to use". If you see just black, its probably because you haven't put anything into OBS yet.


[^1]: Needs OBS 26.1 minimum.
[^2]: Needs OBS 26.1 minimum. Requires v4l2loopback-dkms.
