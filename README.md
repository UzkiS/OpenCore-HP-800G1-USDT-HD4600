<!--
 * @Date: 2021-04-29 14:08:06
 * @LastEditors: LemoFire
 * @LastEditTime: 2021-05-13 16:40:05
 * @FilePath: /OpenCore-HP-800G1-USDT-HD4600/README.md
-->

# OpenCore-HP-800G1-USDT-HD4600

OpenCore for HP 800G1 USDT with HD4600 and Intel WLAN (Perfect config)

## OC information

- OC Version: 0.6.9
- Tested OS Version: 11.3.1 (20E241)

## Working

- WIFI
- Sound

## Not working

> Waiting for you to discover

## Before installation

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

| Name          | Version |
| ------------- | ------- |
| Lilu          | 1.5.3   |
| VirtualSMC    | 1.2.3   |
| WhateverGreen | 1.4.9   |
| AppleALC      | 1.6.0   |
| AirportItlwm  | 2.0.0   |
| IntelMausi    | 1.0.6   |
| USBInjectAll  | 0.7.6   |
