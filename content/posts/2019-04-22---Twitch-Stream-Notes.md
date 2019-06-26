---
title: Twitch Stream Notes - April 22, 2019
date: "2019-04-22T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-04-22-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Bots"
  - "IoT"
description: "Stream for Monday, April 22nd. Continuing the Wall of Things and Twitchbot project."
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/IQFcZeWAjjA" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What we did

### Show and Tell (5 minutes)

- OpenMV Cam
- Sparkfun Apollo Edge Dev Board
- My schedule this week! (no stream Thurs, streaming on the Particle Twitch channel on Friday)

### Continuing the Wall of Things (~1 hour, 55 min)

- Review what we did last time

- Things I want to do in the bot today:
  1. Detect cheers, follows and subs, hosts and trigger fire mode for 10 seconds before returning to the last sequence. 
  2. WoTBot helper command `!bot-help`
  3. Create a `!pulse` command to check my heart rate, on demand
  4. Allow the breathe color to be configurable
  5. Handling an invalid list of colors
  6. Add `!clay` command and trigger disco mode

- Things I want to do in firmware today:
   1. Allow the breathe color to be configurable
   2. Consider ways to sync up the breathe animation
   3. Disco mode

## What we learned / Ideas for next time

- clarkio suggesting using the tmi module types and tslint to check my usage of the tmi.js API
- Check out wappalyzer (via jam3sn_)
- Good discussion on bot testing, check out what theMichaelJolley and clarkio are doing to test their bots.