---
layout: sonoplus
title: Instant Music Library
---

# Instant Music Library

<p style="color:#B8290B">[Experimental feature. This page is a draft; diagrams to follow.]</p>

Your SonoPlus provides a simple to use, zero configuration 'NAS' (Network Attached Storage) feature called **Instant Music Library**.

Instant Music Library allows you to copy your personal music collection to USB memory sticks or other USB storage devices, and add them to your Sonos system as [music libraries](https://support.sonos.com/s/article/257). All the songs in your libraries will be accessible to all Sonos players, and playable via all your Sonos apps.

Your SonoPlus is always-on, so your music library will always be available, without worrying about keeping your computers switched on or having to buy and correctly configure a dedicated NAS just for Sonos.

Instant Music Library creates **read-only** network shares using the older SMB v1 protocol supported by Sonos. 

Up to four USB storage devices can be added. Note that if you're planning to use a USB-attached hard drive, we strongly recommend that you use one with external power, to avoid excessive power demands on the SonoPlus's USB ports.

# Setting up your Instant Library

## Step 1: Prepare the USB storage device

Connect the storage device to your computer, then:

1. Make sure your storage device is formatted as a **FAT32** volume. This is the default format for most devices when they're new, but a reformat may be necessary if it's been changed.
1. Rename your storage device to give it the label **SONOPLUS**, so it can be correctly detected as a music library by your SonoPlus.
1. Copy your music library (or other supported audio files) to the storage device. This may take a while, depending on the size of your library and the speed of your storage device.

## Step 2: Install the USB storage device in your SonoPlus

1. Power-down your SonoPlus
1. Plug in the USB storage to one of the SonoPlus's four USB ports
1. Power-on your SonoPlus

## Step 3: Add your Instant Library to Sonos

You can add your new NAS music library to Sonos using any of the Sonos mobile or desktop controllers. Add it as a network attached share using the following share name:

`\\sonoplus.local\sonoplus1`

Leave the username and password blank.

Once the share has been added, Sonos will automatically start a music library (re)index process. When this is complete, the contents of your USB storage device will be available to play via the Sonos apps.

## Step 4: Additional USB storage devices

You can add up to four USB storage devices at the same time. Prepare them all using the process outlined in Step 1, then they can all be attached while the power is switched off in Step 2. Additional devices can also be added at any time later.

Each separate storage device needs to be added individually in the Sonos music library setup. The names of the additional shares are:

```
\\sonoplus.local\sonoplus2
\\sonoplus.local\sonoplus3
\\sonoplus.local\sonoplus4
```

These names will be used in order, i.e., your second storage device will be shared at `sonoplus2`, and so on.

## Step 5: Making changes

If you need to make changes to your music library, just remove the relevant USB storage device from your SonoPlus, connect it to your computer, and make your desired changes. Once done:

1. Power-down your SonoPlus
1. Re-add the USB device
1. Power-up your SonoPlus
1. Perform a music library reindex, using the Sonos app.

If you remove a USB storage device from your SonoPlus permanently, be sure to perform a music library reindex. Note that device removal can result in your remaining storage devices changing their share name, e.g., a storage device shared as `sonoplus2` might shift to being shared as `sonoplus1`. This could break Sonos playlists and favourites you've created that include tracks from your SonoPlus music libraries, so please **take care when removing devices**!