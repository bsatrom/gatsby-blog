---
title: Twitch Stream Notes - May 09, 2019
date: "2019-05-09T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-05-09-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "Edge ML"
  - "IoT"
  - "ML"
  - "Google Coral"
  - "Particle"
description: "Stream for Thursday, May 09th. Starting an Edge ML and IoT Project with Particle and the Google Coral."
---

- Time: 2-4 pm Central
- VOD [https://www.twitch.tv/videos/422595599](https://www.twitch.tv/videos/422595599)

## What we did

### Show and Tell (15 minutes)

- MOAR AliExpress hardware for the PortaPi Pentester!
- Adafruit buttons and switches!
- [Microsoft BUILD Announcements](https://azure.microsoft.com/en-us/blog/build-with-azure-iot-central-and-iot-plug-and-play/) (Iot Central, IoT Plug and Play)
- Streaming schedule change! Moving to once per week

### Edge ML & IoT Project

- NEW Project: Emotion Mesh! Using the Google Coral and Particle Mesh to do Edge-based face-tracking and emotion detection
- Configure VSCode's new Remote Dev for SSH on the Google Coral Board
  - *Using SSH FS instead as VS Code remote doesn't support ARM-yet*
- Walk through the Coral Object Detection and face-tracking source code
- Create a UART Connection between an Argon and the Coral to start the FT demo (Mesh.sub on Argon, Serial1 to Coral; Coral receives serial, triggers demo; Demo result sent back to Argon over Serial)
  - Resource: [Coral docs](https://coral.withgoogle.com/docs/dev-board/gpio/)
- Set-up a project in Azure IoT Central for Emotion Mesh

## What we learned / Ideas for next time

- Use the medium arcade button, maybe? 
  - @dot_commie and @phrakberg voted for the large button
- Grokking Deep Learning is an awesome book, and there's a [GitHub site for it](https://github.com/iamtrask/Grokking-Deep-Learning)!
- We should be able to use the existing FT source and just capture an image from the webcam to use as the input; This can be extended to use emotion detection inference later
- Brandon needs to catch up on the [Tesla Autonomy Day demos](https://www.youtube.com/watch?v=-b041NXGPZ8)

Next Time! (Monday, May 13th)

- Finish UART Setup
- Set-up Webcam and image capture
- Run FT demo on a captured image