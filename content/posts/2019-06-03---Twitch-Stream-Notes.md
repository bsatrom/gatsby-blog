---
title: Twitch Stream Notes - June 3, 2019
date: "2019-06-03T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-06-03-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "ML"
  - "IoT"
  - "Google Coral"
  - "Particle"
description: "Weekly stream for June 3rd, 2019. IoT Show & Tell, and continuing work on the Google Coral and Particle Powered #EmotionMesh project."
---

- Time: 12-3 pm Central
- VOD [https://www.twitch.tv/videos/433960361](https://www.twitch.tv/videos/433960361)

## What we did

### Show and Tell (15 minutes)

- New Grove Sensors (Speech Recognition and Alcohol)
- Azure Sphere DevKit

### Emotion Mesh! Edge ML & IoT Project (2 hours, 45 minutes)

#### Recap

- Talk about what we did last week
    1. Soldered the Argon to an Adafruit PP board
    2. Updated Coral board to Mendel v3 
    3. Moved the Serial connection to UART3
    4. Auto-mount the SD Card to /disk1 on startup
    5. Trained and tuned a local emotion detection model for the Coral

#### This time
            
- Implement server to client websocket call with image name and emotion result
- Display captured result and toggle off streaming display
- Show graphical result of emotion detection (pie chart?) on web ui
- Prompt user to hit green or red buttons to "vote" on the result
- Capture result from button box and send reset to Web UI

#### Stretch (probably next time)

- Figure out how I am going to capture stats for captures
- Start working on neopixel strips and ultrasonic for triggering the demo

## What we learned

- I need the Myo band maybe... https://smile.amazon.com/Thalmic-Labs-Gesture-Control-Presentations/dp/B00VHWBH02/ref=smi_www_rco2_go_smi_3905707922?_encoding=UTF8&%2AVersion%2A=1&%2Aentries%2A=0&ie=UTF8

- Bot needs to take hsl colors (thanks [@kleinfreund](https://twitch.tv/kleinfreund))
- Bot needs a police command (solid and flashing colors)

## Thanks!

- [@phrakberg](https://twitch.tv/phrakberg) resubbed for 3 mo!
- [@roberttables](https://twitch.tv/roberttables) resubbed for 3 mo!