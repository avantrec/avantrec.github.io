---
layout: sonoplus
title: FAQ
---

# Frequently Asked Questions

## What's included?

The SonoPlus is a compact [Raspberry Pi 3](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/) computer housed in the official red and white Raspberry Pi case. Included are a preinstalled 32GB memory card, an Ethernet cable (2m) and an official Raspberry Pi power supply.

![SonoPlus](/images/20190622-DSC_8894.jpg)

## How do I set up my SonoPlus?

Simply connect the SonoPlus to your network using the Ethernet cable, then plug in the power supply and connect it to the micro-USB power socket on the SonoPlus. That's it.

SonoPlus is a plug-and-play 'appliance', and no end-user configuration or management is required. See [Installation]({{ site.baseurl }}{% link sonoplus/installation.md %}) to learn more.

## How do I use SonoPlus AirPlay?

Your older Sonos players appear as new AirPlay speakers, and they can be used and controlled exactly like any other AirPlay devices. The new SonoPlus speakers are denoted by a plus ('+') after their Sonos room name, e.g.:

![SonoPlus](/images/AirPlayMenu_Smaller.png)

SonoPlus supports multiple simultaneous AirPlay streams from different Apple devices to different Sonos speakers, so you only need one SonoPlus device to support all of your Sonos players.

Speaker volume, play/pause, next/previous track are all controlled by the sending device, as with any other AirPlay speaker.

In the Sonos apps, you'll see that audio is being sent to your Sonos player(s) via your SonoPlus:

![SonoPlus](/images/SonosAppView_Smaller.png)

You can also adjust the speaker volume and stop the audio stream, directly from the Sonos app.

Grouping Sonos players via the Sonos app works in the normal way -- the AirPlay stream will be sent to all of the grouped players, with Sonos managing the synchronised distribution as with any other audio source.

## How does SonoPlus AirPlay work?

SonoPlus uses the open source [AirConnect](https://github.com/philippe44/AirConnect) software project to provide AirPlay (v1) capabilities to all Sonos players. 

SonoPlus detects all Sonos players, and creates AirPlay targets for each of them. When an AirPlay stream is started, SonoPlus acts as a bridge between the AirPlay device and speaker, and converts the audio to a streaming format that Sonos can play.

SonoPlus configures AirConnect to exclude any newer Sonos players that already support AirPlay 2, to avoid any duplication of speakers in the AirPlay menus.

Avantrec contributes to AirConnect's development by submitting code improvements, suggesting feature enhancements, and reporting defects. We also independently test every new AirConnect release before making it available on SonoPlus.

## How's the sound quality?

It's excellent: AirPlay sends audio to SonoPlus in lossless ALAC format, and SonoPlus converts that into lossless FLAC format for playback by Sonos, with no reduction in quality. Hence, the audio quality is as good as the original source, up to and including lossless CD quality.

## Is AirPlay v1 any good?

While it's true that AirPlay v1 has a mixed reputation, it's quite possible for it to work very well. In particular, the AirConnect system installed in SonoPlus allows generous buffering to be configured on both the sending (AirPlay) and receiving (Sonos) streams, to prevent audio dropouts.

{: id="remote-management"}
## How is SonoPlus managed and kept up-to-date? Is it secure?

We use the [Balena](https://www.balena.io) Internet of Things (IoT)  service to manage all SonoPlus devices, including keeping the software secure and functional, as well as adding functionality over time.

This approach has a strong focus on [security](https://www.balena.io/docs/learn/welcome/security/) both in terms of the software that runs on SonoPlus devices as well as the means by which the devices are remotely accessed and managed.

SonoPlus requires an Internet connection to obtain software updates and to permit remote management, using only a secure **outbound** VPN connection. No **inbound** connections from the Internet are required or allowed. Use of the AirPlay function itself doesn't require an Internet connection.

## Which Sonos players are supported?

SonoPlus supports all Sonos players ever produced. This includes the newer players that provide AirPlay 2, but these are detected and omitted by SonoPlus.

## Is SonoPlus for me?

If you want a plug-and-play solution that delivers a reliable and easy to use AirPlay capability for your older Sonos players, then SonoPlus is likely to be a good fit for your needs. 

If you're technically capable and can set up AirConnect on your own Raspberry Pi (or other computer), and keep it up-to-date and working, then it's definitely worth having a go. If you can set up a [Docker](https://blog.docker.com/2019/03/happy-pi-day-docker-raspberry-pi/) environment on a Raspberry Pi, you could use the publicly available AirConnect docker image that we maintain at [Docker Hub](https://hub.docker.com/r/psychlist/docker-airconnect-arm).

## What is SonoPlus *not* good for?

SonoPlus provides AirPlay v1, not v2. This means that it doesn't include the enhancements in v2, such as the ability to synchronise audio with video playback on the sending device.

## Is there a software-only version of SonoPlus?

Not yet, but possibly in the future. We want to control the exact hardware specifications for the time being, to deliver a consistently good experience.

## Why do you use a Raspberry Pi as the basis for SonoPlus?

The Pi is ideally suited for the SonoPlus application. It's small, silent, reliable, has low power demands, and has regulatory approval in all target geographies. And, it's a little computing  powerhouse, with more than enough processing power for the initial AirPlay capability as well as for a range of upcoming new features.

## What's next for SonoPlus?

AirPlay is just the first in a series of Sonos enhancement functions under development for SonoPlus, which is designed to support multiple complementary features as independent software 'slices' that can be enabled and disabled on a per-device basis. New features will be delivered automatically as software updates.

*Any other questions? Please get in touch at [avantrec.ltd@gmail.com](avantrec.ltd@gmail.com)*.