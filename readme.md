
# ASRock Z490M-ITX/ac
- This repo is forked from: https://github.com/Old-Black-Dog/Hackintosh-ASRock-Z490M-ITX-ac. (Credit: Old-Black-Dog@github)
- The origin post on reddit: https://www.reddit.com/r/hackintosh/comments/hl0kbe/asrock_z490itxac_intel_10700k_catalina_155_nzxt/. (Credit: OoJimboO@reddit)

### Spec
- MotherBoard: ASRock z490m-itx/ac
- CPU: i7-10700k
- GPU: AMD 5600XT


### What Works:
- Metal
- Apple Store
- Ethernet (intel 1219v)
- Sleep/Wake
- Sound - Headphones (front), Internal Speaker (rear), Microphone (rear).
- CPU/GPU identified correctly in System Properties
- iMesage/iPhoto/iCloudDrive... ~~(Find My Mac is not working)~~
- FindMyMac worked with BCM94360NG.

### Mostly:
- Bluetooth: (from stock intel ax200 m.2)
  - Enabled by https://github.com/OpenIntelWireless/IntelBluetoothFirmware
    - 20-aug-2020: v1.1.2: Devices have to be turned off/on to reconnect after sleep/reboot
- Wifi(from stock intel ax200 m.2): 
  - Enabled by https://github.com/OpenIntelWireless/itlwm and https://github.com/OpenIntelWireless/HeliPort
    - itlwm kext is not included in this repo since I am moving to a native supported card (BCM94360NG)
    - 20-aug-2020: v1.0.0-alpha: Works, but the speed is quite slow: (100Mpbs@Windows / 10Mbps@MacOS)

#### What doesn't yet
- Ethernet (2.5Gb)

#### Update:
- 21-jul-2020: now using OpenCanopy
- 21-jul-2020: cleaned up kexts, the unused ones now removed
- 21-jul-2020: redid the portmapping through hackintool (kext is now USBPorts.kext)
- 20-Aug-2020: updated OpenCore to 0.6.0
- 08-Sep-2020: 
  - Updated OpenCore to 0.6.1 for iMac 20,1 support 
  - Removed Intel Bluetooth Kext (Because I am using BCM94360NG)
  - Updated AppleALC to 1.5.2
    - Removed WorkAround discribed in https://www.reddit.com/r/hackintosh/comments/i1jzhk/alc1220_not_working_on_z490/ 
    - Updated LiLu.kext to 1.4.7 as the dependency 
  - Fixed DRM
- 20-Dec-2020: updated OpenCore to 0.6.4
- 25-Apr-2021: updated OpenCore to 0.6.8 (Now Working with BigSur)

#### Bios 
- All images (todo:markup relevant changes): [Bios Images](https://github.com/Old-Black-Dog/Hackintosh-ASRock-Z490M-ITX-ac/blob/master/Images/Bios/ASRockz490mitxac_bios_%202020-07-17%2008.28.20.pdf)
