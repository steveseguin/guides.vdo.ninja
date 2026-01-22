---
layout:       post
title:        "Rooms - Two-Way Audio & Video"
date:         2020-12-16 10:00:00 +0000
author:       "Steve Seguin"
categories:   basic
tags:         rooms audio video chat
permalink:    rooms
order:        2

# POSTS LIST
class:       "style2"                         # config bg-color to post list card (1..6)
list-image:  "/assets/screenshots/create-room.png"       # config image to post list card (1..6)
description: >                                # site meta description
  Learn how to create a VDO.Ninja room for two-way audio and video chat. Simple setup for beginners.
list_description: >
  Two-way audio and video, the easy way.

# POST HEADER
header-image: "/assets/screenshots/create-room.png"      # config image to post header
alt-image:    "Creating a room in VDO.Ninja" # config image description to alt att.
---

**Rooms are the easiest way to have a two-way conversation in VDO.Ninja.** When you create a room and share the link, everyone can hear and see each other automatically.

{:.info}
If you want to talk with a remote guest and have them hear you too, use a room! The basic push/view links are one-way only.

## Why Use Rooms?

- **Two-way audio and video** - Everyone in the room can hear and see each other
- **Simple setup** - Just create a room and share one link
- **No custom links needed** - Unlike manual push/view setups, everyone uses the same room link
- **Built-in echo cancellation** - Audio works properly without feedback

## Creating a Room

1. Visit [VDO.Ninja](https://vdo.ninja) in your browser
2. Click **Create a Room**

<figure>
<img src="{{site.url}}/assets/screenshots/create-room.png" title="Create a Room"/>
<figcaption>Click "Create a Room" on the VDO.Ninja homepage</figcaption>
</figure>

3. Enter a room name (or leave it blank for a random name)
4. Click **Enter the Room's Control Center**

## Inviting Guests

Once in your room, you'll see an **Invite a Guest** link. Copy this link and send it to anyone you want to join.

<figure>
<img src="{{site.url}}/assets/screenshots/room-copy-link.png" title="Copy Guest Link"/>
<figcaption>Copy the guest invite link to share with others</figcaption>
</figure>

When your guest opens the link:
- They'll select their camera and microphone
- They'll join the room and see/hear you
- You'll see/hear them

**That's it!** Both of you can now have a two-way conversation.

## Adding Room Video to OBS

To capture the room video in OBS or other streaming software:

1. In the room control center, find the **Add to Scene** button for each guest

<figure>
<img src="{{site.url}}/assets/screenshots/room-add-to-scene.png" title="Add to Scene"/>
<figcaption>Click "Add to Scene" to get the OBS link for a guest</figcaption>
</figure>

2. Copy the scene link that appears

<figure>
<img src="{{site.url}}/assets/screenshots/room-scene-link.png" title="Scene Link"/>
<figcaption>Copy this link into an OBS Browser Source</figcaption>
</figure>

3. In OBS, add a **Browser Source** and paste the link

## Quick Room Links

You can also join a room directly using a simple URL format:

- `https://vdo.ninja/myroom` - Join a room called "myroom"
- `https://vdo.ninja/?room=myroom` - Same thing, different format

Share this link with others and everyone who opens it will be in the same room, able to see and hear each other.

## Next Steps

- Learn about [manual two-person chat](/2personchat) for advanced control over individual streams
- Explore the [full documentation](https://docs.vdo.ninja) for room settings and parameters
