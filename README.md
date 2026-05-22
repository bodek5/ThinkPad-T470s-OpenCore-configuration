# ThinkPad-T470s OpenCore configuration
ThinkPad T470s OpenCore EFI, Monterey -> Tahoe

## What works?
* Graphicts acceleration
* Wifi
* Keyboard & TouchPad & TrackPad
* Sleep option
* Dual-battery
* USB ports
* Brightness & Volume keys
* ThunderBolt
* Camera
* Microphone
* and some more

## Not Working:
* FingerPrint scanner
* Bluetooth (fixable)
* tell me more 

## Working versions:
* Monterey - Working bluetooth, Wi-fi, speakers and other!
* Ventura - Working bluetooth, Wifi speakers and other!
* Sequoia - Working Wi-fi, speakers and other!
* Tahoe - Working Wi-fi, full working sleep option, trying to fix sound!

## Untested:
* Sonoma - I skipped this verion by update from ventura to Sequoia, but it should work
* Versions older than Monterey (someone said they work)

## I NEED PATCH??
Nope, my ThinkPad started all OS without graphicts patching. You only need to install HeliPort app for working Wi-Fi and add it to autostart in Sequoia and higher.

## Thanks to:
* [Dortania](https://github.com/dortania/) for OpenCore
* [acidanthera](https://github.com/acidanthera/) for Lilu.kext and WhateverGreen.kext
* [corpnewt](https://github.com/corpnewt/) for ProperTree
* [openintelwireless](https://github.com/openintelwireless/) for Intel Wi-Fi
