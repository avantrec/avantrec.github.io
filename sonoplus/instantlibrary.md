---
layout: sonoplus
title: Instant Music Library
---

**Important: there is currently a problem in the Sonos S1 (v11.2) and Sonos S2 software versions that is preventing the addition of SonoPlus Music Library shares. Earlier Sonos versions are unaffected.**

# Instant Music Library

SonoPlus provides an easy-to-use, zero configuration, instant 'NAS' (Network Attached Storage) feature called **Instant Music Library**.

Just copy your music collection to a USB memory stick or other USB storage device such as a USB disk, plug it into your SonoPlus, and it's then available for playback on your Sonos system as a [music library](https://support.sonos.com/s/article/257) ![External](/images/external_link.png).

Your SonoPlus is always-on, so your music library will always be available, without worrying about keeping computers connected and switched on, or having to buy and correctly configure a NAS unit just for Sonos. Your SonosPlus creates **read-only** network shares automatically, using the original **SMB v1** protocol required by Sonos.

You can use all four of the SonoPlus's USB sockets to connect USB storage devices, and up to **nine** devices in total can be connected if you use a suitable USB expansion hub.

# Setting Up Your Instant Library

## Step 1: Copy your audio files to the USB storage device

1. **Connect** the USB storage device to your computer
1. Make sure your USB storage device is **formatted** as a **FAT32** volume. This is the default format for most devices when they're new, but a reformat may be necessary if the format has been changed.
1. **Rename** your USB storage device to give it the name/label '**SONOPLUS1**', so it will be identified as containing a music library by your SonoPlus.
1. **Copy your music library** (or other supported audio files) to the USB storage device.
1. **Remove** the USB storage device from your computer.

## Step 2: Install the USB storage device in your SonoPlus

Just insert the USB device into one of the four USB ports on your SonoPlus. The device will be automatically detected and its contents shared on the network within a few seconds.

## Step 3: Add your new Instant Library to Sonos

You can add your new music library to Sonos using any of the Sonos mobile or desktop controller apps, using [music library management](https://support.sonos.com/s/article/257) ![External](/images/external_link.png). Add it as a **Network Device** (NAS) share using the following share name:

**\\\sonoplus.local\sonoplus1**

Leave the username and password **blank**.

Once the share has been added, Sonos will automatically start a music library index process. When this is complete, the contents of your USB storage device will be available to play via the Sonos apps under the **Music Library** section of your system.

This step only needs to be done once for each USB device. You don't need to repeat it if you subsequently remove and reinsert the USB device to make changes.

# Optional Steps

## Making changes to your music library

When you make changes to the music library on a USB device, just:

1. **Remove** the USB storage device from your SonoPlus
1. **Connect** it to your computer, and make your desired changes
1. **Remove** the USB device from your computer and reinsert it into your SonoPlus
1. SonoPlus will re-share the device's contents on the network and **automatically** initiate a Sonos music library reindex to pick up your changes

You **don't** need to power-down your SonoPlus when you add or remove USB devices.

## Installing additional USB storage devices

You can include up to nine USB storage devices on your SonoPlus (subject to using one or more USB hubs to expand the number of USB ports). Prepare them all using the process outlined in **Step 1** above, but **name** the second device **SONOPLUS2**, the third **SONOPLUS3**, and so on.

Follow **Step 2** above when you add storage devices.

Each separate storage device needs to be added individually in the Sonos music library setup. The names of the network shares match the names of the available storage devices, as follows:

- **SONOPLUS2** is shared at **\\\sonoplus.local\sonoplus2**
- **SONOPLUS3** is shared at **\\\sonoplus.local\sonoplus3**

... and so on.

## Permanently removing a USB storage device

If you remove a USB storage device from your SonoPlus *permanently*, remember to remove the folder from the Sonos Music Library folder list using one of the Sonos controller apps.
