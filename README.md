# Kemoge Malware Archive (2015-2016)

WARNING: This repository contains active Android malware from the historical Shedun/Kemoge campaign. It is intended exclusively for reverse engineering, threat signature development, and security research. Do not execute or decompress these files on any physical system or corporate network.

## Archive Configuration
- File Encryption Password: infected
- Format: Password-protected ZIP archive
- Target Operating Systems: Android 4.4 KitKat and Android 5.0 Lollipop frameworks

## Threat Overview
Discovered originally by researchers at FireEye and Lookout in late 2015, the Kemoge threat family represents a sophisticated form of trojanized mobile adware. The operators decompiled popular third-party applications, injected a bundle of up to eight open-source root exploits, and repackaged them for redistribution on alternative storefronts. 

Upon installation, the app registers a custom broadcast receiver inside the AndroidManifest file to trigger silently at boot. It then attempts execution of root commands to permanently embed malicious payloads directly into the read-only /system/app partition. This technique renders the infection permanent against factory resets, allowing it to inject persistent, full-screen ad overlays, capture device configuration values, and silently download secondary malicious packages without user interaction.

## Target Application Catalog
The following variants are bundled within this preservation package:

- Sex Cademy
- Assistive Touch
- Calculator
- Kiss Browser
- Smart Touch
- ShareIt
- Privacy Lock
- Easy Locker
- 2048kg
- Talking Tom 3
- WiFi Enhancer
- Light Browser
