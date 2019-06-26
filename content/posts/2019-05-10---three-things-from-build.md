---
title: Three things I learned about Microsoft's IoT vision at Build
date: "2019-05-10T23:46:37.121Z"
template: "post"
draft: false
slug: "/posts/three-iot-thing-build/"
category: "Conferences"
tags:
  - "Azure"
  - "Microsoft"
  - "IoT"
  - "News"
  - "Conferences"
description: "This week, I attended Microsoft's annual Build conference. It was my first trip back to build since the very first iteration many years ago and I was excited to see Microsoft's vision for developers, up close."
---

![](https://thepracticaldev.s3.amazonaws.com/i/rgspek9xybmg1rr0uxfy.jpg)

**Photo by [Leio McLaren (@leiomclaren) on Unsplash](https://unsplash.com/@leio?utm_medium=referral&amp;utm_campaign=photographer-credit&amp;utm_content=creditBadge)**

This week, I attended Microsoft's annual Build conference. It was my first trip back to build since the very first iteration many years ago—when I was a Microsoft employee and the star of the show was Windows 8!—and I was excited to see Microsoft's vision for developers, up close. 

There were a whirlwind of announcements across the three days in all areas of Microsoft's business, but as a maker and embedded developer, my primary interest was in the company's ever-increasing attention on the IoT. Here are three major things I learned about Microsoft's vision for the IoT from my time at Build.

_Note: The views and opinions expressed here are mine, and do not represent those of my employer, [Particle](https://particle.io). Nor are they meant to indicate any public statement about Particle product features, integrations, roadmap changes or shifts in strategy. This post is merely one developer's opinion and should be treated as such._

## "The Intelligent Edge" is an extension of Microsoft's long commitment to a hybrid cloud computing model 

Satya Nadella's keynote on day one of Build was a tight, two-hour whirlwind that touched on almost every area of Microsoft's business. Nadella framed his remarks around what he referred to as "four distinct platform opportunities" for Microsoft, each of which drove a section of the keynote. They were:

1. Intelligent Cloud & Edge
2. Business Process Automation
3. Office 365
4. Gaming 

The Microsoft CEO made only passing mention of "the IoT" in name during his keynote. Instead, he spent the first segment talking about edge computing, and the role he sees Azure playing in "extending the cloud to the edge." He invoked the term "hybrid cloud" more than a few times, and emphasized that a successful hybrid cloud environment requires "consistency between the cloud and the edge."

### ABInBev and Srarbucks

With those remarks as the frame, Nadella went on to share customers already using Azure to enable this form of edge-to-cloud hybrid computing, including ABInBev and Starbucks. Starbucks had an extensive expo hall demo of their Azure-powered products, including an Azure Machine Learning-powered customized ordering engine (Deep Brew) and an Azure IoT Central And Azure Sphere-powered system for monitoring and management of Starbuck's Mastrena II espresso machines.

![](https://thepracticaldev.s3.amazonaws.com/i/tvt5u0nb8jslqnruvtex.png)
_Starbucks' AzureML powered DeepBrew recommendation system_

![](https://thepracticaldev.s3.amazonaws.com/i/t28eyq1xjr9tmv5zczdd.png)
_Starbucks' white-labeled Azure IoT Central dashboard for espresso machine monitoring_

If you've been a Microsoft-watcher for the last decade, the term "hybrid cloud" will sound familiar. It's one that Microsoft has been using since the very early days of Azure, when Ballmer's vision for hybrid was a mix of public cloud and private cloud compute resources that were seamlessly connected. The idea then was to ease the transition of wary enterprise customers into cloud computing, while enabling those same customers to explore the benefits of elastic compute resources without pivoting solely to the cloud. Whereas Amazon's AWS grew in its early days on the compute needs of startups averse to "owning iron," Microsoft's bread-and-butter was EA-signing enterprises who already had plenty of iron.

Given that history—and as far as I'm aware Microsoft never really pivoted away from this narrative even as Azure has evolved in the last decade—it should come as no surprise that Microsoft sees the "IoT edge" as just another spoke in the hybrid cloud. In this world, your factory, farm, retail store, or truck is its own computing environment, and should sense, actuate and compute seamlessly with the rest of your business.

The "hybrid cloud" is a powerful narrative that I'm sure has served the company well with traditional businesses in the last decade. After Build, I can see how it would be compelling to those same businesses as they pursue somewhat unfamiliar connectivity (read IoT) solutions.

## Scott Guthrie shared the MSFT vision of ML on the edge with options

After Nadella's keynote, the Build audience was invited to choose between two deep dive technical keynotes: one focused on Azure, and another the Office 365 and Dynamics platform. I opted for the Scott Guthrie-helmed Azure keynote, hoping for a bit more depth around the Intelligent Edge and IoT narratives from the keynote.

As with the keynote, Guthrie's session covered a lot of ground, with product announcements and demos across all of the Azure stack and its associated developer tools. In the IoT realm, the conversation was again focused on hybrid cloud computing and their customers increased attention to building solutions that offload processing and decision-making "to the edge." This was especially apparent in amount of attention paid to the demos and solutions that featured an edge Machine Learning (ML) component. It was in that discussion that I learned something interesting about Microsoft's perspective on the edge and IoT.

In the IoT universe of 2019, much of the focus on edge computing—especially as it relates to ML—is how to do ML on the edge using Single Board Computers and Microcontrollers. As SBCs and MCUs get beefier, it's becoming possible to perform ML inference—that is, performing a prediction against a pre-trained model; model training is still in the domain of more powerful computers—on constrained devices. 

In the world of Edge ML products, SBCs and MCUs have dominated. Google's TPU-based [Coral DevBoard](https://coral.withgoogle.com/) and the NVIDIA [Jetson Nano](https://developer.nvidia.com/embedded/buy/jetson-nano-devkit) are two examples of recently-released Pi-like SBCs with ML inference skills. SparkFun has released an [Edge MCU](https://www.sparkfun.com/products/15170) that runs TensorFlow lite models, and the [announcement just this week](https://os.mbed.com/blog/entry/uTensor-and-Tensor-Flow-Announcement/) at Google I/O of a unification between the [TensorFlow Lite](https://www.tensorflow.org/lite/) and [uTensor](https://github.com/utensor/) projects are strong signals that MCU-based inference is a reality.

However, Microsoft seems to view edge ML a bit differently. The company didn't announce an ML-capable SBC or MCU at Build, nor did they disparage the existence of these products as frivolous. Instead, where much of the ML narrative of today seems to be heading toward a continuum of training in the cloud and inference on constrained devices, Microsoft painted a picture where a third computing option sits in the middle: one of edge servers and stacks that offload training from the cloud and inference from devices, while offering the same speed and security that makes edge ML so enticing in the first place. 

In floor demos and videos, they featured products like the Azure Stack, a rack of FPGA-powered cards for edge processing, the Azure DataBox for ingesting data by the terabyte into the cloud, and the [Vision AI DevKit](https://azure.github.io/Vision-AI-DevKit-Pages/#). The latter is probably the closest thing to an SBC-style ML device that Microsoft has, but even it was featured working in concert with other, higher-powered edge devices.

The featured floor demo in this space was from Kroger, who is using the Vision AI DevKit, Azure Stack and DataBox Edge to perform out-of-stock detection on supermarket shelves without needing to backhaul streaming video to the cloud for ML processing and inference.

![](https://thepracticaldev.s3.amazonaws.com/i/eag3m1il5ipj8axozwx2.png)
_A mockup booth of the Kroger stock detection system._

Microsoft didn't explicitly paint this story as an either-or between ML-capable SBCs or MCUs and their products, and they may very well have a product or two in the works as we speak. But one thing that was apparent to me is that when Microsoft thinks about the edge and the hybrid cloud, they think their customers need a variety of options to choose from when building IoT solutions, not just ML-capable SBCs/MCUs.  

## Microsoft's vision of the IoT is plug-and-play

Perhaps you noticed that Microsoft made a few product announcements in the days and weeks leading up to Build this year. There's one [you might have missed](https://azure.microsoft.com/en-us/blog/intelligent-edge-innovation-across-data-iot-and-mixed-reality/) as it was buried under a few others: IoT Plug and Play.

I saw the [announcement when it dropped the Thursday before Build[](https://azure.microsoft.com/en-us/blog/intelligent-edge-innovation-across-data-iot-and-mixed-reality/), but I'll admit that I was skeptical. I read the announcement, and took a quick scan around the Azure IoT Device Catalog, but the entire thing felt like a marketing ploy to me: clever naming, but little news of value for the IoT developer.

Turns out, I was wrong. In a few sessions from Sam George, Peter Provost and Briton Zurcher on Monday and Tuesday, I realized that the Plug and Play naming was more than branding. As it turns out, a plug and play model might just be exactly what the IoT needs to make solution development easier.

Think about a typical IoT solution of today. You select an MCU or SBC to be the brains of the project, then populate it with sensors and actuators to do something. In some cases, you might even buy a self-contained product like a dashcam or streaming video camera and connect it directly to Wi-Fi. You write firmware to interface with devices, and then you connect the product and its various sensors and actuators to the cloud.

Often, this step of wiring a physical product up to a cloud solution is the challenging part. Connectivity, security and messaging (MQTT, TCP, AMQP, etc.) aside, even the act of defining the telemetry data that your solution will capture and send, or the cloud to device commands it responds to requires manual work in firmware and in cloud solutions like Azure IoT Central.

[IoT Plug and Play](https://azure.microsoft.com/en-us/blog/build-with-azure-iot-central-and-iot-plug-and-play/) is Microsoft's open source, standards-based answer to this problem. The secret sauce here is a JSON-LD schema called a Device Capability Model, which can be used to define device metadata like who makes it, what firmware version it's running, what telemetry it sends and collects, and what cloud-side commands it responds to. Here's an example of a capability model from the [capability model spec](https://github.com/Azure/IoTPlugandPlay/tree/master/DTDL):

```javascript
{
    "@id": "http://example.com/thermostatDevice/1.0.0",
    "@type": "CapabilityModel",
    "displayName": "Thermostat T-1000",
    "implements": [
        {
            "@id": "http://example.com/thermostat/1.0.0",
            "@type": "Interface",
            "displayName": "Thermostat",
            "contents": [
                {
                    "@type": "Telemetry",
                    "name": "temp",
                    "schema": "double"
                },
                {
                    "@type": "Property",
                    "name": "setPointTemp",
                    "writable": true,
                    "schema": "double"
                }
            ],
            "@context": "http://azureiot.com/v0/contexts/Interface.json"
        },
        "http://azureiot.com/interfaces/deviceInformation/1.1.3"
    ],
    "@context": [
        "http://azureiot.com/v0/contexts/CapabilityModel.json",
        "http://azureiot.com/v0/contexts/Interface.json"
    ]
}
```

The advantage of a capability model like this is that it creates a contract between the disparate systems in an IoT solution. It can be plugged into a SaaS product like Azure IoT Central and recognize telemetry and commands automatically. It can be used to generate C/C++ code to collect telemetry or respond to commands. It can even be used by developer tools and IDEs (like VS Code) to auto-generate capability models based on implementation-specific firmware.

![](https://thepracticaldev.s3.amazonaws.com/i/ryitk3hqpm3diwppo44b.png)
_An overview of how IoT Plug and Play enables various aspects of the solution development process._

And much as Plug and Play of 90s-era Microsoft Windows enabled consumers to buy third-party peripherals and trust that they would "just work," IoT Plug and Play seeks to enable the same experiences for IoT solution builders and device manufacturers alike. And because the [underlying definition language is open source](https://github.com/Azure/IoTPlugandPlay), I'm quite hopeful that this will be picked up and leveraged well-beyond the Microsoft ecosystem.

I meet a lot of makers, embedded and hardware engineers in my work for Particle. One of the things we often find ourselves saying to each other is that there's never been a better time to do what we do. Dev kits are cheaper than ever; resources abound on places like [YouTube](https://www.youtube.com/channel/UCpYjkSkGOXAMXeZjZkbb-PQ), [Twitch](https://twitch.tv/brandonsatrom), [Hackster](https://hackster.io), and [Hackaday](https://hackaday.io); IoT vendors like [Particle](https://particle.io) continue to build simple, secure and scale-ready platforms; and [Adafruit](https://adafruit.com) is there to make sure we never stop having fun while building things.

If you're looking to solve a real-world problem in the IoT space, there's never been a better time to dig in. Microsoft seems to agree, and after what I've seen this week, I think all of us working in this space stand to benefit, now and in the future.
