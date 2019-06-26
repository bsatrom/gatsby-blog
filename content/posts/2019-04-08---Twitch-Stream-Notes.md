---
title: Twitch Stream Notes - April 8, 2019
date: "2019-04-08T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-04-08-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Bots"
  - "IoT"
description: "Stream for Monday, April 8th. Continuing the Wall of Things and Twitchbot project."
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ns6I7ObrGwg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What we did

### Show and Tell (10 minutes)

- Adafruit PyPortal
- MxChip IoT DevKit
- Jetson Nano Developer Kit

### Continuing the Wall of Things (1 hour, 45 min.)

- Review what we did last time
- Off stream, I updated all four strips to respond to the new `setColors` function on the gateway.

- Things I want to do in the bot today:
  1. Add support for Hex colors
  2. Set colors even when the chase command is active
  3. Add the `!stop` command
  4. Change the mode to `!rainbow`
  5. Detect cheers, follows and subs and trigger a fireworks (or disco mode as per [cooperCLAY](https://www.twitch.tv/cooperCLAY)) animation on all strips, in sync.

- Things I want to do in firmware today:
  1. Add support for Hex colors
  2. Add a fireworks/pulse animation mode for bits/subs, etc.

## What we learned / Ideas for next time

- [ProfessorStrawberry](https://www.twitch.tv/ProfessorStrawberry) asked about the power draw of the devices on the Wall. We should measure that.
- The left LED strip appears to be mis-calibrated (or needs to be replaced)
- Accept CSS shorthand values ([parithon](https://www.twitch.tv/parithon)'s idea) [ex. `#FFF` = `#FFFFFF`, `#FC0` = `#FFCC00`] 
- Accept named colors ([dot_commie](https://www.twitch.tv/dot_commie)'s idea) [i.e. cyan, salmon, magenta]
- The LTE gateway is dropping too much; Switch to an Argon (Wi-Fi) for prototyping.
- Many thanks to [parithon](https://www.twitch.tv/parithon) for the five gifted subs!
- Thanks to [parithon](https://www.twitch.tv/parithon), [cpayette](https://www.twitch.tv/cpayette), [cooperCLAY](https://www.twitch.tv/cooperCLAY) for subscribing!
- Thanks to [roberttables](https://www.twitch.tv/roberttables) and [cpayette](https://www.twitch.tv/cpayette) for the cheers!