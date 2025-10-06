# Dolby Atmos Razer Phone 2 Magisk Module

## DISCLAIMER
- Dolby apps and blobs are owned by Dolby™.
- The MIT license specified here is for the Magisk Module only, not for Dolby apps and blobs.

## Descriptions
- Equalizer sound effect ported from Razer Phone 2 (bolt) and integrated as a Magisk Module for all supported and rooted devices with Magisk
- Changes/spoofs ro.product.brand to razer, ro.product.device to bolt, ro.product.manufacturer to Razer, & ro.product.model to Phone 2 which may break some system apps and features functionality
- Global type sound effect
- Conflicted with `vendor.dolby.hardware.dms@2.0-service`

## Sources
- https://dumps.tadiphone.dev/dumps/razer/bolt bolt-user-9-P-SMR1-RC008-ATT-190626-3239-release-keys
- libswvqe.so: LENOVO TB-J606F https://t.me/c/1331480009/94136
- libhidlbase.so, libhidltransport.so, & libhwbinder.so: CrDroid ROM Android 13
- libutils.so: LineageOS 23 Android 16 BP2A.250605.031.A2 1758630651
- libmagiskpolicy.so: Kitsune Mask R6687BB53

## Screenshots
- https://t.me/androidryukimodsdiscussions/66464

## Requirements
- arm64-v8a architecture
- Android 9 (SDK 28) and up
- Magisk or KernelSU installed (Recommended to use Magisk Delta/Kitsune Mask for systemless early init mount manifest.xml if your ROM is Read-Only https://t.me/ryukinotes/49)

## WARNING!!!
- Possibility of bootloop or even softbrick or a service failure on Read-Only ROM if you don't use Magisk Delta/Kitsune Mask.

## Installation Guide & Download Link
- Recommended to use Magisk Delta/Kitsune Mask https://t.me/ryukinotes/49
- Remove any other else Dolby MAGISK MODULE with different name (no need to remove if it's the same name)
- Reboot
- If you have Dolby in-built in your ROM, then you need to activate data.cleanup=1 at the first time install (READ Optionals bellow!)
- Install this module https://www.pling.com/p/1531576/ via Magisk app or KernelSU app or Recovery if Magisk installed
- Install AML Magisk Module https://t.me/ryukinotes/34 only if using any other else audio mod module
- If you are using KernelSU, you need to disable Unmount Modules by Default in KernelSU app settings
- Reboot
- If you are using KernelSU, you need to allow superuser list manually all package name listed in package.txt (and your home launcher app also) (enable show system apps) and reboot afterwards
- If you are using SUList, you need to allow list manually your home launcher app (enable show system apps) and reboot afterwards
- If you have sensors issue (fingerprint, proximity, gyroscope, etc), then READ Optionals bellow!

## Optionals
- https://t.me/ryukinotes/8
- Global: https://t.me/ryukinotes/35
- Stream: https://t.me/ryukinotes/52

## Troubleshootings
- https://t.me/ryukinotes/10
- https://t.me/ryukinotes/11
- Global: https://t.me/ryukinotes/34

## Support & Bug Report
- https://t.me/ryukinotes/54
- If you don't do above, issues will be closed immediately

## Credits and Contributors
- @HuskyDG
- https://t.me/viperatmos
- https://t.me/androidryukimodsdiscussions
- @HELLBOY017
- You can contribute ideas about this Magisk Module here: https://t.me/androidappsportdevelopment

## Sponsors
- https://t.me/ryukinotes/25


