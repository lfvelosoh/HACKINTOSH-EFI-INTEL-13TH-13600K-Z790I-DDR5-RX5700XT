# HACKINTOSH-EFI-INTEL-13TH-13600K-B760M-DDR5-RX5700XT

> 🔧 OpenCore Version: `0.9.8`
>
> 🖥️ SmBIOS: `iMacPro1,1`
> 
> 🍏 MacOS Version: `Sonoma 14.3.1`

## Hardware
| Component       | Model                                    |
|-----------------|------------------------------------------|
| CPU             | Intel Core i5 13th - 13600k              |
| Mainboard       | Maxsun iCraft Z790ITX WIFI               |
| GPU             | AMD Radeon RX5700 XT - 8GB (Asus TUF)    |
| Memory          | XPG Lancer DDR5@5200 MHz - (2x16Gb)      |
| Wireless Card   | Intel Wi-Fi 6E AX211 - 160 MHz           |
| Audio Codec     | ALC897                                   |
| Storage         | KingSpec NMVE NE2280 PCIe Gen3 x4       |

#### Works / Don't Works
|||
|---|---|
|USB Map|✅|
|Custom ACPI Tables|✅|
|Boot Shine|✅|
|Built-in Network cards|✅|
|Built-in Sound cards|✅|
|CPU Name|✅|
|GPU Name|✅|
|WIFI / Bluetooth|✅|
|AirDrop|🚫|
|Sleep|🚫|

## Kexts used (included)
Kext|Description
----|----
[AirportItlwm](https://github.com/OpenIntelWireless/itlwm/releases)|Adds support for a large variety of INTEL WIRELESS cards and works natively in recovery thanks to IO80211Family integration.
[IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)| Adds Bluetooth support to macOS when paired with an Intel wireless card.
[BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM/releases)|Used for uploading firmware on Broadcom Bluetooth chipset, required for all non-Apple/non-Fenvi Airport cards.
[Lilu.kext](https://github.com/acidanthera/Lilu/releases)|Patch many processes, required for AppleALC, WhateverGreen, VirtualSMC and many other kexts.
[SMCProcessor.kext](https://github.com/acidanthera/VirtualSMC/releases)|Used for monitoring CPU temperature.
[SMCSuperIO.kext](https://github.com/acidanthera/VirtualSMC/releases)|Used for monitoring fan speed.
[VirtualSMC.kext](https://github.com/acidanthera/VirtualSMC/releases)|Emulates the SMC chip found on real macs, without this macOS will not boot.
[WhateverGreen.kext](https://github.com/acidanthera/WhateverGreen/releases)|Used for graphics patching, DRM fixes, board ID checks, framebuffer fixes, etc; all GPUs benefit from this kext.
[AppleALC.kext](https://github.com/acidanthera/AppleALC/releases)|Used for AppleHDA patching, allowing support for the majority of on-board sound controllers.
[LucyRTL8125Ethernet.kext](https://www.insanelymac.com/forum/files/file/1004-lucyrtl8125ethernet/)|For Realtek's 2.5Gb Ethernet.
[NVMeFix.kext](https://github.com/acidanthera/NVMeFix/releases)|Used for fixing power management and initialization on non-Apple NVMe.
[RestrictEvents.kext](https://github.com/acidanthera/RestrictEvents/releases)|Better experience with unsupported processors like AMD, Disable MacPro7,1 memory warnings and provide upgrade to macOS Monterey via Software Updates when available.
[CpuTscSync.kext](https://github.com/acidanthera/CpuTscSync/releases)|It is a Lilu plugin, combining functionality of VoodooTSCSync and disabling xcpm_urgency if TSC is not in sync. It should solve some kernel panics after wake.
[USBMap.kext](https://github.com/corpnewt/USBMap)|Kext generated after mapping the USB ports

## Tools

Tool|Description
:----|:----
[ProperTree](https://github.com/corpnewt/ProperTree) | Configure config.plist
[USBMap](https://github.com/corpnewt/USBMap) | Making the USB Map
[gibMacOS](https://github.com/corpnewt/gibMacOS) | Download and create macOS images
[SSDTTime](https://github.com/corpnewt/SSDTTime) | Make creating SSDTs simple
[CPU-Name](https://github.com/corpnewt/CPU-Name) | Fix the cpu name
[MountEFI](https://github.com/corpnewt/MountEFI) | Shortcut to Mount the EFI Driver
[gibMacRecovery](https://github.com/corpnewt/gibMacRecovery) | Download and create macOS recoverys
[gebSMBIOS](https://github.com/corpnewt/GenSMBIOS) | Generate information from SMBIOS
[IORegistryExplorer](https://github.com/vulgo/IORegistryExplorer) | Validate information regarding hardware power management
[iASL](https://www.acpica.org/downloads) | Change and convert SSDTs (for Windows)
[Mac iASL](https://github.com/acidanthera/MaciASL) | Change and convert SSDTs (for MAC)
[OpenCore-Packager](https://github.com/chris1111/OpenCore-Packager) | Tool that assists in the installation of the EFI in a simple way

> ## Softwares
> - [Stats](https://github.com/exelban/stats)
> - [Hackintool](https://github.com/benbaker76/Hackintool)

>## Useful Links
>- [Dortania Getting Started](https://dortania.github.io/getting-started/)
>- [Dortania Troubleshooting](https://dortania.github.io/troubleshooting/)
>- [Dortania Post Install](https://dortania.github.io/OpenCore-Post-Install/)
>- [Dortania Documentation](https://dortania.github.io/docs/)
>- [Original repository](https://github.com/luchina-gabriel/BASE-EFI-INTEL-DESKTOP-13THGEN-14THGEN-RAPTOR-LAKE-PUBLIC)

> ## Warnings ⚠️
> - Always install using a wired network
> - Configure AppleID only at the end of the process
> - With every change in EFI after installation, make a backup.
> - Command to validate if the kexts are running → `kextstat | greep-v com.apple`
> - Command to disable unauthorized app blocking → `sudo spctl —master -disable`
