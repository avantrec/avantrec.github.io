---
layout: sonoplus
title: Instant Music Library
---

# Instant NAS Music Library

Your SonoPlus provides an easy-to-use, zero configuration, instant 'NAS' (Network Attached Storage) feature called **Instant Music Library**.

Just copy your music collection to a USB stick, plug it into your SonoPlus, and it's then available for playback on your Sonos system as a [music library](https://support.sonos.com/s/article/257).

A single, large capacity, 256GB USB memory stick (now available for about $25) can hold at least 500 CDs of CD quality losslessly encoded music, or at least 1,500 CDs encoded as 320kbps MP3, so you can support an extensive music library with your SonoPlus and simple, inexpensive storage devices.

Your SonoPlus is always-on, so your music library will always be available, without worrying about keeping your computers switched on or having to buy and correctly configure a dedicated NAS just for Sonos: Instant Music Library creates **read-only** network shares using the SMB v1 protocol required by Sonos.

Up to nine USB storage devices (memory sticks or hard drives) can be added to your SonoPlus. Note that if you're planning to use a USB-attached hard drive, we strongly recommend that you use one with external power, to avoid excessive power demands on the SonoPlus's USB ports. The same applies if you choose to add an external USB hub.

# Setting up your Instant Library

## Step 1: Prepare your USB storage device

Connect the USB storage device to your computer, then:

1. Make sure your storage device is **formatted** as a **FAT32** volume. This is the default format for most devices when they're new, but a reformat may be necessary if the format has been changed.
1. **Rename** your storage device to give it the name/label **SONOPLUS1**, so it can be  identified as a music library by your SonoPlus.
1. **Copy your music library** (or other supported audio files) to the storage device. This may take a while, depending on the size of your library and the speed of your storage device.

## Step 2: Install the USB storage device in your SonoPlus

1. Power-down your SonoPlus
1. Plug in the USB storage device to one of the SonoPlus's four USB ports
1. Power-on your SonoPlus

## Step 3: Add your Instant Library to Sonos

You can add your new NAS music library to Sonos using any of the Sonos mobile or desktop controllers. Add it as a network attached (NAS) share using the following share name:

**\\\sonoplus.local\sonoplus1**

Leave the username and password blank.

Once the share has been added, Sonos will automatically start a music library (re)index process. When this is complete, the contents of your USB storage device will be available to play via the Sonos apps under **Music Library**.

## Step 4: Making changes

If you need to make changes to your music library, just remove the relevant USB storage device from your SonoPlus, connect it to your computer, and make your desired changes. Once done:

1. Power-down your SonoPlus
1. Re-add the USB device
1. Power-up your SonoPlus
1. Perform a music library reindex, using the Sonos app.

If you remove a USB storage device from your SonoPlus permanently, be sure to perform a music library reindex otherwise the music on the removed device will still appear in your Sonos library.

## Step 5: Additional USB storage devices

You can include up to nine USB storage devices on your SonoPlus. Prepare them all using the process outlined in **Step 1** above, but **name** the second device **SONOPLUS2**, the third **SONOPLUS3**, and so on.

Follow **Step 2** above When you add or remove storage devices.

Each separate storage device needs to be added individually in the Sonos music library setup. The names of the network shares match the names of the available storage devices, as follows:

- **SONOPLUS2** is shared at **\\\sonoplus.local\sonoplus2**
- **SONOPLUS3** is shared at **\\\sonoplus.local\sonoplus3**
- ... and so on.