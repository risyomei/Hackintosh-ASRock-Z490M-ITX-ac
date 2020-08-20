
# ASRock Z490M-ITX/ac
- This repo is forked from: https://github.com/Old-Black-Dog/Hackintosh-ASRock-Z490M-ITX-ac. (Credit: Old-Black-Dog@github)
- The origin post on reddit: https://www.reddit.com/r/hackintosh/comments/hl0kbe/asrock_z490itxac_intel_10700k_catalina_155_nzxt/. (Credit: OoJimboO@reddit)

# Spec
- MotherBoard: ASRock z490m-itx/ac
- CPU: i7-10700k
- GPU: AMD 5600XT


### What Works:
- Metal
- Apple Store
- Ethernet (intel 1219v)
- Sleep/Wake
- Sound - Headphones (front), Internal Speaker (rear), Microphone (rear)  (via FakePCIID patch kext).
- CPU/GPU identified correctly in System Properties
- iMesage/iPhoto/iCloudDrive... (Find My Mac is not working)

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

#### Bios 
- All images (todo:markup relevant changes): [Bios Images](https://github.com/Old-Black-Dog/Hackintosh-ASRock-Z490M-ITX-ac/blob/master/Images/Bios/ASRockz490mitxac_bios_%202020-07-17%2008.28.20.pdf)
