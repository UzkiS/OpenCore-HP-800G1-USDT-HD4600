# OpenCore-HP-800G1-USDT-HD4600

HP 800G1 USDT with HD4600‘s OpenCore for MacOS 11
(为什么是 11 因为 12 系统 HD4600 有显示毛边问题，老老实实呆在 11 养老吧)

2022/4/12 本仓库根据 800G1 DM 的 OC 例行更新一下，今后主要在 [OpenCore-HP-800G1-DM-HD4600](https://github.com/LemoFire/OpenCore-HP-800G1-DM-HD4600) 仓库更新，DM 与 USDT 的区别主要就是 ReleaseUsbOwnership 的值为 False，还有 nvmefix 的 kext，还是那句话，机子坏了没办法测试，无法使用请下载 releases 中的 [BigSur-1.0](https://github.com/LemoFire/OpenCore-HP-800G1-USDT-HD4600/releases/tag/BigSur-1.0)，这个历史版本是实机测试过的，本仓库今后不会再更新了

如果这个版本没问题的话，相比之前修复了 2K 分辨率问题，4K 不要想了，除非你的板子没有锁死 VRAM，这个时候可以自己尝试修改

## OC information

_(Note that due to the damage of my machine, this version of EFI has not been tested on the machine. If it cannot be used, please download BigSur-1.0)_

- OC Version: 0.7.9
- Tested OS Version: 11.6.5 (20G527)

## Tested

- 2K screen resolution
- Double screen (resolution: 3440\*1440@60Hz + 1920\*1080@120Hz)（已经设置了最优的显存分配，再调高会出现花屏问题，将就一下了）
- Sleep

## Not working

- Unknow

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

| Name                                                                | Version |                                                                                                          |
| ------------------------------------------------------------------- | ------- | -------------------------------------------------------------------------------------------------------- |
| [Lilu](https://github.com/acidanthera/Lilu)                         | 1.6.0   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/Lilu)             |
| [VirtualSMC](https://github.com/acidanthera/VirtualSMC)             | 1.2.9   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/VirtualSMC)       |
| [WhateverGreen](https://github.com/acidanthera/WhateverGreen)       | 1.5.8   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/WhateverGreen)    |
| [AppleALC](https://github.com/acidanthera/AppleALC)                 | 1.7.0   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/AppleALC)         |
| [AirportBrcmFixup](https://github.com/acidanthera/AirportBrcmFixup) | 2.1.4   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/AirportBrcmFixup) |
| [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)         | 2.6.1   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/BrcmPatchRAM)     |
| [IntelMausi](https://github.com/acidanthera/IntelMausi)             | 1.0.7   | ![GitHub release (latest by date)](https://img.shields.io/github/v/release/acidanthera/IntelMausi)       |
