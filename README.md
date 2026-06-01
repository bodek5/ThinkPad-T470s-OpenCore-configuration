# ThinkPad-T470s OpenCore configuration
ThinkPad T470s OpenCore 1.0.7 EFI, Monterey --> Tahoe

## What works?
* Graphicts acceleration
* Wifi
* Bluetooth (on Monterey and Ventura)
* Backlight on keyboard
* Keyboard & TouchPad & TrackPad
* Sleep option
* Dual-battery
* USB ports
* Brightness & Volume keys
* ThunderBolt
* Microphone
* and some more

## Not Working:
* FingerPrint scanner
* camera (little bug who will be fixed on 1.3)
* tell me more 

## HOW TO FIX NATIVE WI-FI FOR SEQUOIA
* Mount your EFI partition
* Open config.plist on ProperTree
* Search #PciRoot(0x0)/Pci(0x1C,0x2)/Pci(0x0,0x0) and delete hashtag (#)
* Reboot
* Open OpenCore Legacy Pather
* patch network card
* reboot
* add hashtag back to PciRoot(0x0)/Pci(0x1C,0x2)/Pci(0x0,0x0)
* reboot
* if not working - reset nvram and reboot
* Now your wifi will work nativelly, its better for battery life and apps compatibility

## RECOMMECTED
I recommend to install Sequoia over other all, runs fast (need to turn off spotlight and siri + leave it turn on for 1h or more to end indexing, in first hours performance will be bad), has new layout, battery works fine, and its stable + i work on sequoia more than others (so i patch bugs more often)

## NOTE FOR TAHOE
If you run Tahoe on T470s, you need to know that speakers ,camera, microphone and bluetooth do not work unless you patch them yourself (you can patch speakers by voodooHDA, but volume control work bad), the battery will be drained and the performance will be weaker, after an hour of running Tahoe, the laptop will speed up a bit and animations will stop stuttering because indexing will finish, but the overall performance and battery are much worse than Sequoia because of the liquid glass. On my T470s fans always on..., also wi-fi looks like be slower.

## Working versions:
* Monterey - Working native Wi-fi, Bluetooth, speakers, sleep and other!
* Ventura - Working native Wi-fi, Bluetooth, speakers, sleep and other! 
* Sequoia - Working native Wi-fi, speakers, sleep and other!
* Tahoe - Working Wi-fi (HeliPort), sleep, not working cam,mic,bt, wifi slower.

## Untested:
* Sonoma - I skipped this verion by update from ventura to Sequoia, but it should work
* Versions older than Monterey (someone said they work)

## I NEED PATCH??
Only on Sequoia for native Wi-Fi, and maybe tahoe but i dont tested it yet. other things like graphicts acceleration dont need patching, its working fully on all versions.

## Thanks to:
* [Dortania](https://github.com/dortania/) for OpenCore
* [acidanthera](https://github.com/acidanthera/) for Lilu.kext, WhateverGreen.kext and VirtualSMC.
* [corpnewt](https://github.com/corpnewt/) for ProperTree and genSMBIOS
* [openintelwireless](https://github.com/openintelwireless/) for Intel Wi-Fi and Bluetooth
* [MultimediaLucario](https://github.com/MultimediaLucario/) for BATC.aml (from T470) (Dual-Battery aml)
* [zhen-zen](github.com/zhen-zen/) for YogaSMC
