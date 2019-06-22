---
layout: sonoplus
title: FAQ
---

# Frequently Asked Questions

## What's included?

The SonoPlus is a [Raspberry Pi 3](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/) computer housed in the official red and white Raspberry Pi case. Included are a preinstalled 32GB memory card, an Ethernet cable (2m) and an official Raspberry Pi power supply.

![SonoPlus](/images/20190622-DSC_8894.jpg)

## How do I set up my SonoPlus?

Simply connect the SonoPlus to your network using the Ethernet cable. Then, plug in the power supply and connect it to the Micro-USB power socket on the SonoPlus. That's it.

SonoPlus is an 'appliance', and no end-user configuration or management is required.

## How do I use SonoPlus AirPlay?

Your older Sonos players appear as new AirPlay speakers, and they can be used and controlled exactly like any other AirPlay devices. The SonoPlus speakers are denoted by a '+' after their Sonos room name, e.g.:

![SonoPlus](/images/AirPlayMenu_Smaller.png)

SonoPlus supports multiple simultaneous AirPlay streams from different Apple devices to different Sonos speakers, and works with speakers that are grouped via the Sonos app.

Speaker volume, play/pause, next/previous track are all controlled by the sending device, as with any other AirPlay speaker.

In the Sonos apps, you'll see that audio is being sent to your Sonos player(s) via your SonoPlus:

![SonoPlus](/images/SonosAppView_Smaller.png)

## How does the SonoPlus AirPlay feature work?

SonoPlus uses the open source [AirConnect](https://github.com/philippe44/AirConnect) software project to provide AirPlay version 1 capabilities to all Sonos players. 

SonoPlus detects all Sonos players, and creates AirPlay targets for each of them. If an AirPlay stream is started, SonoPlus acts as a bridge between the AirPlay device and speaker, and converts the audio to a streaming format that Sonos can play.

SonoPlus configures AirConnect to exclude any newer Sonos players that already support AirPlay 2, to avoid any duplication of speakers in the AirPlay menus.

Avantrec contributes to AirConnect's development by submitting code improvements, suggesting feature enhancements, and reporting defects. We also independently test every new AirConnect release before making it available on SonoPlus.

## How's the sound quality?

It's excellent: AirPlay sends audio to SonoPlus in lossless ALAC format, and SonoPlus converts that into lossless FLAC format for playback by Sonos, with no reduction in quality. Hence, the audio quality is as good as the original source, up to and including lossless CD quality.

## Is AirPlay version 1 any good?

While it's true that AirPlay v1 has a mixed reputation, it's quite possible for it to work very well indeed. In particular, the AirConnect code used by SonoPlus allows the use of generous buffering -- on both the sending and receiving streams -- to prevent audio dropouts.

## How is SonoPlus managed and kept up-to-date? Is it secure?

Avantrec uses the [Balena](https://www.balena.io) Internet of Things (IoT)  service to manage all SonoPlus devices, including keeping the software secure and functional, as well as adding functionality over time.

This approach has a strong focus on [security](https://www.balena.io/docs/learn/welcome/security/) both in terms of the software that runs on SonoPlus devices as well as the means by which the devices are remotely accessed and managed.

SonoPlus requires an Internet connection only for remote management and software updates. The AirPlay function itself doesn't require an Internet connection.

## Is SonoPlus for me?

If you want a plug-and-play solution that delivers a reliable and easy to use AirPlay capability for your older Sonos players, then SonoPlus is likely to be a good fit for your needs.

If you're technically capable and can set up AirConnect on your own Raspberry Pi (or other computer), and keep it up-to-date and working, then it's definitely worth a try.

## What is SonoPlus *not* good for?

SonoPlus provides AirPlay v1, not v2. This means that it doesn't include the enhancements in v2, such as the ability to synchronise audio with video playback on the sending device.

## Is there a software-only version of SonoPlus?

Not yet, but possibly in the future. We want to control the exact hardware specifications for the time being, to deliver a consistently good experience.

*Any other questions? Please get in touch at [avantrec.ltd@gmail.com](avantrec.ltd@gmail.com)*.