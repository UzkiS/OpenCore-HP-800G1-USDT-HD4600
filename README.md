<!--
 * @Date: 2021-04-29 14:08:06
 * @LastEditors: LemoFire
 * @LastEditTime: 2021-08-03 14:33:20
 * @FilePath: /undefined/Users/lemofire/Documents/git/OpenCore-HP-800G1-USDT-HD4600/README.md
-->

# OpenCore-HP-800G1-USDT-HD4600

OpenCore for HP 800G1 USDT with HD4600

## OC information
*(Note that due to the damage of my machine, this version of EFI has not been tested on the machine. If it cannot be used, please download BigSur-1.0)*
- OC Version: 0.7.2
- Tested OS Version: 11.5.1 (20G80)
- Tested resolution: 1920\*1080

## Working

- WIFI(Intel or Broadcom(no wireless card test))
- Sound
- USB Port

## Not working

- 4K (BIOS settings are not very compatible)

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

| Name                                                                | Version         |
| ------------------------------------------------------------------- | --------------- |
| [Lilu](https://github.com/acidanthera/Lilu)                         | 1.5.5           |
| [VirtualSMC](https://github.com/acidanthera/VirtualSMC)             | 1.2.6           |
| [WhateverGreen](https://github.com/acidanthera/WhateverGreen)       | 1.5.2           |
| [AppleALC](https://github.com/acidanthera/AppleALC)                 | 1.6.3           |
| [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)          | 2.0.0(2021-8-2) |
| [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) | 2.1.3           |
| [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)         | 2.6.0           |
| [IntelMausi](https://github.com/acidanthera/IntelMausi)             | 1.0.7           |
| [USBInjectAll](https://github.com/Sniki/OS-X-USB-Inject-All)        | 0.7.6           |
