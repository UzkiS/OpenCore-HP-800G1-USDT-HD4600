<!--
 * @Date: 2021-04-29 14:08:06
 * @LastEditors: LemoFire
 * @LastEditTime: 2021-06-08 14:16:01
 * @FilePath: /undefined/Users/lemofire/Documents/git/OpenCore-HP-800G1-USDT-HD4600/README.md
-->

# OpenCore-HP-800G1-USDT-HD4600

OpenCore for HP 800G1 USDT with HD4600 and Intel WLAN

## OC information

- OC Version: 0.7.0
- Tested OS Version: 11.4 (20F71)

## Working

- WIFI
- Sound
- USB Port(fixed on 0.7.0)

## Not working

- 4K (No equipment for testing, if you have one, you can submit PR)

## Before installation

**star this project ( > ω < )**

***Don't try to use the VGA port to boot!***

#### Edit config.plist

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

| Name          | Version |
| ------------- | ------- |
| Lilu          | 1.5.3   |
| VirtualSMC    | 1.2.4   |
| WhateverGreen | 1.5.0   |
| AppleALC      | 1.6.1   |
| AirportItlwm  | 2.0.0   |
| IntelMausi    | 1.0.6   |
| USBInjectAll  | 0.7.6   |
