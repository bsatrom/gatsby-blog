---
title: Twitch Stream Notes - April 11, 2019
date: "2019-04-11T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-04-11-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Bots"
  - "IoT"
description: "Stream for Thursday, April 11th. Continuing the Wall of Things and Twitchbot project."
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/aX3S_3AtNJ8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What we did

### Show and Tell (5 minutes)

- Green screen!

### Continuing the Wall of Things (1 hour, 45 min.)

- Review what we did last time

- Things I want to do in the bot today:
  1. accept CSS shorthand values (ex. expand `#fc0` into `#ffcc00`)
  2. Accept named colors (ex. cyan, magenta, red, green, blue, salmon)
  3. Detect cheers, follows and subs and trigger a fireworks (or disco mode as per [cooperCLAY](https://www.twitch.tv/cooperCLAY)) animation on all strips, in sync.
  4. Add a `!breathe` command

- Things I want to do in firmware today:
  1. Install a beta version of v0.9.1 on the Argon to improve gateway reliability 
  2. Implement disco mode for bits/subs, etc.
  3. Implement a pulse/breathe mode

## What we learned / Ideas for next time

- I need to add a `!lurk` command to chat
- dot_commie suggested using [TinyColor](https://bgrins.github.io/TinyColor/) for CSS and named color handling in the bot and it is awesome!
- Consider adding alternating colors to the chase animation
- Controller still timing out, but it seems to happen when chase mode or color changes are triggered
- Found an [awesome collection of LED Strip animations](https://www.tweaking4all.com/hardware/arduino/adruino-led-strip-effects/#LEDStripEffectFadeInandFadeOutRedGreenandBlue) with support for both NeoPixel and FastLED!