---
title: Twitch Stream Notes - June 10, 2019
date: "2019-06-10T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-06-10-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "ML"
  - "IoT"
  - "Google Coral"
  - "Particle"
description: "Weekly stream for June 10rd, 2019. Continuing work on the Google Coral and Particle Powered #EmotionMesh project."
---

- Time: 12-3 pm Central
- VOD 

## What we did

### Emotion Mesh! Edge ML & IoT Project

#### Recap

- Talk about what we did last week
    1. Completed overall demo flow on UI
    2. Added local storage for run results
    3. Added charts and stats to UI

#### This time
            
- Add a Xenon-powered Neopixel strip to the network
- Mesh Publish state changes from controller to network
- Mesh subscribe to state changes on Neopixels
- Add an attract animation on Idle
- Add a processing animation
- Add a waiting animation
- Add an inference correct animation
- Add an inference incorrect animation

## What we learned

- You can update the brightness on Neopixels at runtime, just need to call `strip.show()` for the change to be picked up. ALSO pass AND USE your `brightness` variable. :kappa:

## Thanks!

- https://twitter.com/SlenderSherbet/status/1138158034809737218
- @cooperClay resubbed for 3 mo
- @nick_larsen raided with 5 viewers
- @bscolaro Came in and gave a public service announcement about heat and caring for your pets