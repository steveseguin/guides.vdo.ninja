---
layout:       post
title:        "VDO.Ninja basics"
date:         2020-12-16 10:00:00 +0000
author:       "Steve Seguin"
categories:   basic
tags:         basics
permalink:    basics
order:        1

# POSTS LIST
class:       "style1"                         # config bg-color to post list card (1..6)
list-image:  "/assets/images/pic01.jpg"       # config image to post list card (1..6)
description: >                                # site meta description
  Learn what tech powers VDO.ninja, and quickly get up and running.
list_description: >
  If lost, start here.


# POST HEADER
header-image: "/assets/screenshots/Site.png"      # config image to post header
alt-image:    "VDO.Ninja landing page" # config image description to alt att.
---

VDO.Ninja needs 2 thinks to work:
  - Someone pushing a video feed out from their device
  - Someone viewing that video feed

1.Visit VDO.Ninja with your web browser (Chrome, Edge, Safari)

2.Click `Add your camera to OBS`

3.Select your camera and audio device from the list of devices

<figure>
<img src="{{site.url}}/assets/screenshots/camera-picker.jpg" title="Camera picker"/>
<figcaption>Camera picker window in VDO.Ninja</figcaption>
</figure>

You will see the video feed of the device on screen, and at the top of the screen a 'view' link.

Copy this view link and send it to someone you want to have access to this feed, or place it inside a 
OBS browser source.

<img src="{{site.url}}/assets/screenshots/view-link.jpg" title="View Link"/>

<img src="{{site.url}}/assets/images/obs.jpg" title="browser source"/>

## Cheat Sheet

A printable quickstart guide can be found here:<br />
<img src="https://github.com/steveseguin/vdoninja/raw/quickstart/basicconcepts/OBSN_basic_concepts.jpg" title="basic cheat sheet" />

## Powered by WebRTC

[WebRTC](https://webrtc.org/)[^1] is the magic behind VDO.Ninja. While the magic sauce is so much more than that, WebRTC powers the engine.
This way VDO.Ninja works everywhere there is a modern browser. MS Edge, Google Chrome, Mozilla Firefox, Safari, Opera, Vivaldi, Brave. You name it.


{:.warning}
VDON is a peer-to-peer system. This means for each new person viewing your feed, a new encode is processed. It also is CPU bound since encoding usually takes place on the CPU. Take care not to overload your system. Keep an eye on your CPU usage.

[^1]: Web Real-Time Communication
