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
- libmagiskpolicy.so: Magisk (stable) 30.7 (30700)

## Changelog

v1.0.5
- Check functions in mirror /apex files instead of mirror /system if exist
- Remove hardware services conflict restart (Use this instead: https://github.com/reiryuki/Hardware-Services-Restarter-Magisk-Module)
- Fix sepolicy denial

v1.0.4
- Fix inaccessible libhwbinder.so in some ROMs
- Removes conflicted weird modules

v1.0.3
- Support NoMount metamodule
- Resets module folders/files permissions at post-fs-data
- Move _uninstall.log to /data/adb/logs/
- Hides LunarisDolby.apk

v1.0.2
- Update libmagiskpolicy.so from Magisk (stable) 30.7 (30700) (fixes selinux denials in KernelSU)
- Does not disable raw playback (You can use Audio Compatibility Patch Reborn Magisk Module instead)

v1.0.1
- Fix wrong target in latest KernelSU
- Improve detections

v1.0.0
- Fix wrong manifest.xml location patch target in latest Magisk version

v9.9
- Tidy up aml.sh
- Exclude \*audio\*effects\*haptic\*.xml
- Fix wrong file permissions in some ROMs

v9.8
- Fix ZN7android8String16aSEOS0 function not found in some ROMs
- Add libutils.so as system_support
- Abort installation if fail to mount mirror system

v9.7
- Fake Kitsune Mask detection
- Improve /odm and /my_product support detection

v9.6
- Fix script bug at installation for libsqlite.so detections
- Fix selinux denials

## Screenshots
https://t.me/androidryukimodsdiscussions/66464

## Requirements
- arm64-v8a architecture
- Android 9 (SDK 28) and up
- HIDL audio service
- Magisk or Kitsune Mask or KernelSU or Apatch installed (Recommended to use Magisk Delta/Kitsune Mask for systemless early init mount manifest.xml if your ROM is Read-Only https://t.me/ryukinotes/49)

## WARNING!!!
Possibility of bootloop or even softbrick or a service failure on Read-Only ROM if you don't use Magisk Delta/Kitsune Mask.

## Installation Guide & Download Link
- Recommended to use Magisk Delta/Kitsune Mask https://t.me/ryukinotes/49
- Remove any other else Dolby MAGISK MODULE with different name (no need to remove if it's the same name)
- Reboot
- If you are using KernelSU, you need to disable Unmount Modules by Default in KernelSU app settings and install https://github.com/KernelSU-Modules-Repo/meta-overlayfs or https://github.com/KernelSU-Modules-Repo/magic_mount_rs or https://github.com/KernelSU-Modules-Repo/hybrid_mount or https://github.com/maxsteeel/nomount first depending on ROM compatibility
- If you have Dolby in-built in your ROM, then you need to activate data.cleanup=1 at the first time install (READ Optionals bellow!)
- Install this module https://devuploads.com/kgc1e6f940tp via Magisk app or Kitsune Mask app or KernelSU app or Apatch app or Recovery if Magisk or Kitsune Mask installed
- Install AML Magisk Module https://t.me/ryukinotes/34 only if using any other else audio mod module
- Reboot
- If you are using KernelSU, you need to allow superuser list manually all package name listed in package.txt (and your home launcher app also) (enable show system apps) and reboot afterwards
- If you are using SUList, you need to allow list manually your home launcher app (enable show system apps) and reboot afterwards
- If you have vibrator, camera, charging/USB, SIM card/RIL, display, brightness, WiFi, thermal, and sensors issues (fingerprint, proximity, gyroscope, etc.), then install https://github.com/reiryuki/Hardware-Services-Restarter-Magisk-Module also

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
- https://t.me/androidappsportdevelopment

## Sponsors
https://t.me/ryukinotes/25


