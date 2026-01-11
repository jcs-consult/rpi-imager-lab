# Home Assistant Lab Image --- Student Guide

## Overview

This guide explains how to flash, boot, and access the Home Assistant
Lab Image used in this course.

## Requirements

-   Raspberry Pi 3B or 4
-   microSD card (16 GB or larger)
-   Power supply
-   Ethernet cable (recommended for first boot)
-   Computer with Raspberry Pi Imager 2.0.0+

## Step 1 --- Install Raspberry Pi Imager

Download from https://www.raspberrypi.com/software/

## Step 2 --- Configure Custom Repository

1.  Open Raspberry Pi Imager
2.  App Options → Content Repository → Custom URL
3.  Paste:
    https://raw.githubusercontent.com/jcs-consult/rpi-imager-lab/main/repo.json
4.  Restart Imager

## Step 3 --- Flash SD Card

Choose OS → HA Lab (Clean) -- 32-bit (Pi 3/4) Choose Storage → SD card
Write

## Step 4 --- Set Device Name (Optional)

On the boot partition, create ha-node.txt with content like: ha-lab-03

## Step 5 --- Boot the Pi

Insert SD card, connect Ethernet, power on. Wait 2--3 minutes.

## Step 6 --- Find IP and Access Home Assistant

Use your router's connected devices list to find the Pi IP. Open:
http://`<PI-IP>`{=html}:8123

.local may work on some networks but IP is authoritative.

Disable VPNs if access fails.

## Step 7 --- Complete Onboarding

Create user and finish setup in browser.

## Adding Wi-Fi Later

sudo nmcli device wifi connect "`<SSID>`{=html}" password
"`<PASSWORD>`{=html}"

## Notes

Ethernet is preferred. Wi-Fi is automatic fallback. Each device is
uniquely identified on first boot.
