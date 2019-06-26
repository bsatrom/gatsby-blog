---
title: Twitch Stream Notes - March 28, 2019
date: "2019-03-28T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/twitch-stream-03-28-2019/"
category: "Twitch Streams"
tags:
  - "Twitch"
  - "Stream Notes"
  - "ML"
  - "IoT"
  - "Google Coral"
  - "Bots"
description: "Stream for Thursday, March 28th. Playing with the Google Coral and continuing the Wall of Things project."
---

🚠 **Going on a ski trip with the family from March 29-April 5. No regular streams next week!** ⛷

## What we did

### Google Coral Object Detection Demo! (15 min)

- Using the [instructions here](https://coral.withgoogle.com/tutorials/devboard-camera/) I want to hook a logitech camera up to the Coral Dev Board and run a few demos (face tracking, object classification)
- SSH into the board, and run this command to make sure the USB camera is connected
  ```
  v4l2-ctl --list-formats-ext --device /dev/video1`
  ```
  
- Download the object classification and image detection models and labels
- Run the object classification model using a streaming server. (Bump down the resolution and FPS a bit from the default command)

```bash
edgetpu_classify_server \
--source /dev/video1:YUY2:640x480:20/1  \
--model ${TEST_DATA}/mobilenet_v2_1.0_224_quant_edgetpu.tflite \
--labels ${TEST_DATA}/imagenet_labels.txt
```

- Run the face detection model using a streaming server. (Bump down the resolution and FPS a bit from the default command)

```bash
edgetpu_detect_server \
--source /dev/video1:YUY2:640x480:20/1  \
--model ${TEST_DATA}/mobilenet_ssd_v2_face_quant_postprocess_edgetpu.tflite
```

### Continuing the Wall of Things (1 hour, 45 min)

- Review what we got working last time
- Off stream, I moved the command if statements into a command object to save us on if/switch mess

- Things I want to do in the bot today:
  1. Use the user/context object to add the chatting username to response messages.
  2. Fix online command to show actual, online `connected: true` devices (currently its every one I own)
  3. Add the `!chase-color` command to set the light color 
      - we decided to add this to the chase command
  4. Add the `!chase-stop` command
  5. Detect cheers, follows and subs and trigger a fireworks animation on all strips, in sync.

- Things I want to do in firmware today:
  1. Make the chase color function settable.
  ```js
  { "red": 23, "green": 50, "blue": 25 }
  ```

  2. Add a fireworks/pulse animation mode for bits/sub commands.


## What we learned

- I will miss you all next week!
- [OpenThread](https://openthread.io) is the mesh networking stack built into Particle 3rd generation devices
- Less trouble context-switching between C++ and JS, although I am still a much better JS developer... 
- [dot_commie](https://twitch.tv/dot_commie) [has a gist](https://gist.github.com/jaredpsimpson/eb212181d1edd4e7f7411fc8b93a66b4) that will allow us to convert hex to RGB next time
- [VICTORY](https://clips.twitch.tv/CarefulHeartlessCucumberUWot)! 
- Didn't get through everything today. Unchecked stuff slides into the next stream!