<!--
 * @Date: 2021-04-29 14:08:06
 * @LastEditors: LemoFire
 * @LastEditTime: 2021-07-06 13:01:33
 * @FilePath: /undefined/Users/lemofire/Documents/git/OpenCore-HP-800G1-USDT-HD4600/README.md
-->

# OpenCore-HP-800G1-USDT-HD4600

OpenCore for HP 800G1 USDT with HD4600 and Intel WLAN

## OC information

- OC Version: 0.7.1
- Tested OS Version: 11.5.1 (20G80)
- Tested resolution: 1920*1080

## Working

- WIFI
- Sound
- USB Port

## Not working

- 4K (No equipment for testing, if you have one, you can submit PR)

## Before installation

### star this project ( > ω < )

### Edit config.plist

**At first, please complete the 'PlatformInfo' by yourself.** [https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#platforminfo)

- PlatformInfo>Generic>MLB
- PlatformInfo>Generic>ROM
- PlatformInfo>Generic>SystemSerialNumber
- PlatformInfo>Generic>SystemUUID

### BIOS Settings

#### Disable

- Fast Boot -> Disabled
- Secure Boot -> Disabled
- Security -> VTd -> Disabled

#### Set

- Storage -> Storage Options -> SATA Emulation > AHCI

## Kext information

| Name                                                          | Version         |
| ------------------------------------------------------------- | --------------- |
| [Lilu](https://github.com/acidanthera/Lilu)                   | 1.5.4           |
| [VirtualSMC](https://github.com/acidanthera/VirtualSMC)       | 1.2.5           |
| [WhateverGreen](https://github.com/acidanthera/WhateverGreen) | 1.5.1           |
| [AppleALC](https://github.com/acidanthera/AppleALC)           | 1.6.2           |
| [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)    | 2.0.0(2021-7-2) |
| [IntelMausi](https://github.com/acidanthera/IntelMausi)       | 1.0.7           |
| [USBInjectAll](https://github.com/Sniki/OS-X-USB-Inject-All)  | 0.7.6           |
