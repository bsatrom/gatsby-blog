---
title: Twitch Stream Notes - April 18, 2019
date: "2019-04-18T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-04-18-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Bots"
  - "IoT"
  - "ML"
  - "NVidia Jetson Nano"
description: "Stream for Monday, April 18th. Exploring the NVidia Jetson Nano Edge ML device; Continuing the Wall of Things and Twitchbot project."
---

- Time: 2-4 pm Central
- VOD [https://www.twitch.tv/videos/412975252](https://www.twitch.tv/videos/412975252)

## What we did

### Show and Tell (5 minutes)

- Particle Workbench is GA, y'all!
- PhaseDock
- Capture Card for things! 

### Start exploring the NVIDIA Jetson Nano (~30 min)

- Already have an SD Card with the image loaded up.
- Connect it to Ethernet and a second display, keyboard and mouse (capture via capture card).
- Check out the docs and read a few demos.

### Continuing the Wall of Things (~1 hour, 30 min)

- Review what we did last time

- Things I want to do in the bot today:
  1. Detect cheers, follows and subs, hosts and trigger fire mode 
  2. Create a `!pulse` command to check my heart rate, on demand
  3. Allow the breathe color to be configurable
  4. Handling an invalid list of colors

- Things I want to do in firmware today:
   1. Update the Argon firmware to Device OS 1.0+
   2. Allow the breathe color to be configurable
   3. Consider ways to sync up the breathe animation

## What we learned / Ideas for next time

- Learn about working with least squares on nonlinear models (thanks @jekensik17)
- Add `!clay` command and trigger disco mode on the lights
- WoTBot helper command `!help`