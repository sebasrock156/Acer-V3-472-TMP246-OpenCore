# Acer Aspire E5-572G/TravelMate P246-MG Hackintosh OpenCore (Monterey 12.2-12.6)

[AppleALC Support Codecs]: https://github.com/acidanthera/AppleALC/wiki/Supported-codecs
[Wireless Support]: https://openintelwireless.github.io/itlwm/Compat.html#dvm-iwn
[DOWNLOAD HERE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/releases/tag/12-releases
[SEE THE GUIDE]: https://github.com/sebasrock156/Acer-E5-572-TMP246-OpenCore/tree/Monterey/GUIDE.md


![progress](https://img.shields.io/badge/progress-done-blue.svg)
![3Dgraphics](https://img.shields.io/badge/3Dgraphics-in_build-blue.svg)
![periphericals](https://img.shields.io/badge/periphericals-working-green.svg)
![installation](https://img.shields.io/badge/installation-working-green.svg)

![img](https://i.imgur.com/NPnWBrz.png)

If do you want try to build your own EFI:
**[SEE THE GUIDE]**

If do you want test EFI from easy way:
**[DOWNLOAD HERE]**

**Now, the hardware**:

Hardware | Model
--- |:--:
![processor](https://i.imgur.com/hWNvzxy.png) | Core i7 5500U 2 Cores/4 Threads @2,4Ghz
![igpu](https://i.imgur.com/ywW6onH.png)| HD 5500 2GB VRAM @900Mhz
![audio](https://i.imgur.com/A7RRuUn.png) | Realtek ALC283
![dgpu](https://i.imgur.com/1frTIg4.png) | GeForce 820M (Not supported on MacOS)
![wlan](https://i.imgur.com/9eDLwo9.png) | Dual Band AC 3160 (From E5-471G)
Ethernet | Realtek RTL8168
---

<details>
 
**Now, some minimum hardware recommendations**:

---

Hardware | Model
--- |:--:
RAM | Any Samsung, Hynix or Kingston DDR3 8GB(4GBx2).
Audio Card | Any Realtek Audio Card (some Broadcom cards may not work).
WLAN Card | Any Intel network card (A few Realtek cards works externally; Intel supported cards is listed below).
SATA Drive	| Any Solid State Drive (SSD) with 240GB of storage.
IDE Drive | Add a caddy for SATA Output, then, I recommend any Hard Disk with 500GB/1000GB of storage.
---
 
</details>

## Works：

<details>
 
Opencore Bootloader 0.9.2 ✅
 
Integrated Graphics ✅ (taken as HD 6000 by system) 

Native Screen ✅ (1366x768) 

Multi Screen ✅ (Native + Any up 3840x2160) 

RJ45 Ethernet Connection ✅
 
USB Ports ✅ (2.0, 3.0/3.1) 

Touchpad ✅ (It's partially working, some gestures may not work; If you use dual boot, touchpad may not work on Windows/BSD for ACPI changes; works fully on linux with xf86-input)
 
HDMI ✅ (Works fully, HDMI Audio works too).

VGA ✅

Camera ✅
 
Card Reader ✅ (Now it's works; Realtek Card readers only) 

Keyboard shortcuts ✅ (At least, volume, touchpad and brightness control; hibernate, and network may not work)

Screen Backlit ✅ (Backlight work as in Linux distros)
**For using brightness control: pressing "Pause" (up backlit ☀+) and "Lock Scroll" (down Backlit ☼-)**.
 
Audio Card ✅ (Now it's fixed *thanks to Alejandro Barreiro from Hackintosh Hispanic 2.0 telegram group*, change "alcid" bootflag *In config.plist --> NVRAM --> Add --> 7C436110-AB2A-4BBB-A880-FE41995C9F82 --> boot-args* for the supported coded for you audio hardware, see in [AppleALC Support Codecs]; If you have problems with some Realtek Audio Card, pull a request here in Github).

Battery Stats & Charge level ✅ (But for ACPI modifications, may have some of battery drain, doesn't show up)

Hibernate ✅ (If you did Dualboot with Windows, works partially in this OS)
 
Bluetooth ✅ (Fully working; this EFI build is for Intel Cards only).

Wi-Fi ✅ (Always that you have an Intel Dual Band *support table below*):

## Supported WLAN Cards (by Intel):
---

Generation | Models
---|:--:
3xxx | Dual Band AC 3160, Dual Band AC 3165, Dual Band AC 3168
4xxx | Dual Band AC 4165
7xxx | Dual Band AC 7260, Dual Band AC 7265
8xxx | Dual Band AC 8260, Dual Band AC 8265
9xxx | Dual Band AC 9260, Dual Band AC 9461, Dual Band AC 9462, Dual Band AC 9560 
---
This EFI use Airportitlwm for fix Wi-Fi connection, see newer hardware in [Wireless Support]
 
</details>


## Working Apps:

Adobe Creative Cloud 2022 (almost all works) ✅

Davinci Resolve 18 ✅

Origin ✅

OBS Studio ✅

Office 2019 ✅

Opera GX ✅

---

## Partially work:

Apple ID's apps ✅❌ (you need to fix SMBIOS)
 

 
