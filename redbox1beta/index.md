---
layout: default
title: Redbox 1 Beta
---

# Avantrec Redbox 1

## What is Redbox 1?

**Redbox 1** from **Avantrec** is a simple plug and play appliance that enhances the Sonos user experience. Its initial focus is to provide **AirPlay** capabilities for all your older Sonos players (the ones that didn't benefit from the introduction of AirPlay 2 support by Sonos).

![Redbox 1](/images/raspberrypi-in-case-01-300px.png)

Redbox 1 is a standard Raspberry Pi 3 computer, housed in the offical Raspberry Pi case. Its software is preconfigured and automatically kept up to date. It's very simple to install: just connect it to your network with an Ethernet cable and plug in its power supply. The capabilities of Redbox 1 will grow over time as new features are added.

Every Redbox 1 is supplied ready to use, with an Ethernet cable and a power supply, and software preinstalled on a memory card.

## AirPlay on the RedBox 1

AirPlay allows Apple devices to send audio output to remote speakers. Newer Sonos players now include AirPlay 2 support, but older players are unsupported, or require awkward workarounds like grouping with a newer speaker, and muting it.

Redbox 1 provides **direct** AirPlay 1 support for all older Sonos players. You just choose the Sonos player you want to use in the normal Apple AirPlay menu, and your audio is sent to the player as with any other AirPlay speaker.

All Sonos players are supported, including the 'ZP' devices, the Connect, Connect:Amp, Play:1, Play:3, and first generation Play:5.

Redbox 1 works by acting as a bridge between the sending Apple device and the receiving Sonos player. Audio is sent in full lossless quality, and Redbox 1 supports several simultaneous AirPlay streams. Redbox 1 makes use of the open source [AirConnect](https://github.com/philippe44/AirConnect) utility to achieve its goals.

## Redbox 1 Management and Support

It's important that the software running on your Redbox 1 is kept up to date, to benefit from new features and improvements, and to keep it secure. Redbox 1 is remotely managed and updated using secure services from [Balena](https://www.balena.io). It requires no end-user software maintenance.

## Installing Redbox 1

To install, simply connect your Redbox 1 to your router (or other attached network switch) with the supplied Ethernet cable. Plug in the power supply, and connect the (micro USB) power connector. That's it. Redbox 1 will take a few minutes to boot, and possibly download the most up to date software. Once that's done, your Sonos players will appear in your AirPlay menus.

Note that your RedBox 1 does require a working Internet connection to allow for software updates and remote management.

***

## Using AirPlay

Sonos players enabled by Redbox 1 will appear in your AirPlay menus, with '+' signs appended to the Sonos room names for the players. They work just like other AirPlay (v1) targets: simply choose the Sonos player you want, and that's where the audio from the Apple device will be sent.

![AirPlay Menu](/images/AirPlayMenu_Smaller.png)

In the Sonos app, you'll now see that the player is receiving its audio stream from AirConnect. You can control what's played, and the volume, all from the sending app.

![AirConnect](/images/Room_Smaller.png)

The Sonos app can be used to group speakers as with any other audio source. All grouped speakers will receive the AirPlay stream.

*Feedback? Questions? Get in touch at [avantrec.ltd@gmail.com](mailto:avantrec.ltd@gmail.com)*