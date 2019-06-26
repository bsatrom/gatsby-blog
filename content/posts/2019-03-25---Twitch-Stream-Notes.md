---
title: Twitch Stream Notes - March 25, 2019
date: "2019-03-25T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-03-25-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "IoT"
  - "Bots"
  - "Brew Buddy"
description: "Stream for Monday, March 25th, 2019. Wrapping up the Brew Buddy project and starting on the Wall of Things project."
---

<iframe width="560" height="315" src="https://www.youtube.com/embed/nlnMwSmlD-w" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## What we did

### Wrapping up Brew Buddy (1 hour)

- Review [submitted PR to electric-io](https://github.com/noopkat/electric-io/pull/107)
    - It was merged, yay!
- Planing to go through a few final issues this morning and then move onto a NEW project:
    1. Turn off TFT in sleep mode 
        - *Turns out, I need to bodge the BL pin on the TFT into the Argon to try this. Plan to look into it off-stream.*
    2.  Double-check my battery reading logic
        - *This looked ok, so we didn't change it*
    3. Double check fermentation rate logic
        -  *A single knock was being detected as multiple, so I implemented a "debounce" to filter out knocks that happen too close together.*

  *It's been fun working on Brew Buddy, but its time to move on...*

### Starting the Wall of Things (1 hour)

- NEW Project: [The Wall of Things!!!](https://github.com/bsatrom/wall-of-things)
    - Plan is to take this pegboard wall and add a 24x7 camera (and public website) to it
    - Over time, I want to to add a number of sensors and projects to this (Happy Plant, panel, servo arm, etc.)
        - We'll add Brew Buddy to this wall as well for automated testing
    - Today, we're going to start a Twitch chatbot to control the Neopixel strips
    - Walk through what the [Neopixel strips do now](https://github.com/bsatrom/wall-of-things/tree/master/wot-firmware/wot-neopixel-strips)
    - Start working on the chatbot
        1. Use [TMI.js](https://docs.tmijs.org/v1.2.1/index.html)
        2. New node project (npm init)
        - [X]  Put it in the [WoT Repo](https://github.com/bsatrom/wall-of-things/tree/master/wot-bot) - *sticking with the monorepo approach here... for now*
    - Features added
      1. Connect the cyanpandabot
      2. Listen for `connected` and `message` events
      3. Display the number of devices I have online
      4. Start the Mesh chase animation with the `!chase` command
      5. Roll the `!dice`

## What I learned

- TMI.js is awesome! 🤖
- The particle-js-api is also awesome! 💙
- Context switching between C++ and JavaScript == (or ===) Brandon makes mistakes! 🤣
- Building a chatbot is ⚡️️️️️️⚡️