# ThinkPad-T470s OpenCore configuration
ThinkPad T470s OpenCore EFI, Monterey --> Tahoe

## What works?
* Graphicts acceleration
* Wifi
* Keyboard & TouchPad & TrackPad
* Sleep option
* Dual-battery
* Bluetooth (sonoma and lower)
* USB ports
* Brightness & Volume keys
* ThunderBolt
* Camera
* Microphone
* and some more

## Not Working:
* FingerPrint scanner
* tell me more 

## NOTE FOR TAHOE
If you run Tahoe on T470s, you need to know that speakers, camera, microphone and bluetooth do not work unless you patch them yourself, the battery will be drained and the performance will be weaker, after an hour of running Tahoe, the laptop will speed up a bit and animations will stop stuttering because indexing will finish, but the overall performance and battery are much worse than Sequoia because of the liquid glass. On my T470s fans always on..., also wi-fi looks like be slower.

## Working versions:
* Monterey - Working Wi-fi, speakers and other!
* Ventura - Working Wifi speakers and other! 
* Sequoia - Working Wi-fi, speakers and other!
* Tahoe - Working Wi-fi, full working sleep option, not working cam,mic,speakers,bt, wifi slower.

## Untested:
* Sonoma - I skipped this verion by update from ventura to Sequoia, but it should work
* Versions older than Monterey (someone said they work)

## I NEED PATCH??
Nope, my ThinkPad started all OS without graphicts patching. You only need to install HeliPort app for working Wi-Fi and add it to autostart in Sequoia and higher.

## Thanks to:
* [Dortania](https://github.com/dortania/) for OpenCore
* [acidanthera](https://github.com/acidanthera/) for Lilu.kext, WhateverGreen.kext and VirtualSMC.
* [corpnewt](https://github.com/corpnewt/) for ProperTree
* [openintelwireless](https://github.com/openintelwireless/) for Intel Wi-Fi
* [MultimediaLucario](https://github.com/MultimediaLucario/) for BATC.aml (from T470) (Dual-Battery aml)
* [zhen-zen](github.com/zhen-zen/) for YogaSMC
