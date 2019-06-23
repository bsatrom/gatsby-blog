---
title: Twitch Stream Notes - May 20, 2019
date: "2019-05-20T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-03-20-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "ML"
  - "IoT"
  - "Google Coral"
  - "Particle"
description: "Weekly stream for May 20th, 2019. IoT Show & Tell, and continuing work on the Google Coral and Particle Powered #EmotionMesh project."
---

# May 20, 2019 Stream

- Time: 12-3 pm Central
- VOD

## What we did

### Show and Tell (15 minutes)

- Personal news update!
- New Edge ML Hardware (Avent Branium and an STM32 Discovery Eval Board)
- Pololu 12V Step-Up Voltage Regulators
- The button box is assembled!

### Emotion Mesh! Edge ML & IoT Project (2 hours, 45 minutes)

#### Recap

- Talk about what we did last time (Set-up cloud-based emotion detection with the Azure Cognitive Services Face API)
- Review what I did last week off-stream
    1. Extended the default video streaming demo to capture a single frame when a button is clicked
    2. Call the Azure Face API from the captured frame
    3. Store results on an SD card and clean-up local resources
    4. Working on training a local emotion detection model for the Coral

#### This time
            
1. Set-up an Argon as a gateway on a new mesh network
2. Set-up firmware projects in the emotion-mesh repo
3. Configure UART communication between Coral and Argon
4. Send a serial message to the Coral when a button on the box is pressed
5. Connect the Arcade buttons to my Gateway Argon and 12v step-up converters
6. Trigger a screen capture and cloud detection from a UART message received on the Coral

#### Stretch (probably next time)

1. Start implementing the emotion training model onto the Coral
2. Set-up a project in Azure IoT Central for Emotion Mesh

## What we learned
- CircuitPython may be available on the Coral. Look into this.
- See if I can find a teardown for the Oura ring (thanks for the idea @bscolaro!)


## Thanks!

- Groguard for the 4-month resub!
- jam3sn_ for 50 bits!