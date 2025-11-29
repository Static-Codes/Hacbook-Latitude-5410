# Notes:
This is **not a plug and play solution** for you to run MacOS Sequoia on your Dell Latitude 5410.

**This configuration is currently semi functional, the operating system works, but it has a few significant bugs/unpatched features**.

Please **do not** use this repository for **anything** other than **occasional references**; for **ALL** questions, please refer to *[Dortania's Guide on Open Core](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)*

Since this laptop is my daily driver and, I'm triple booting on the same SSD, I have chose not to add macOS to my internal EFI partition, instead opting to carry around a few flashdrives with identical copies of my bootloader; This is completely unnecessary for users not intended to dual or triple boot with Windows and MacOS.
## Laptop Specs – Latitude 5410 (P98G007)

| Component            | Specification                                                                |
| ----------------- | ------------------------------------------------------------------ |
| CPU | i5-10210U  |
| iGPU | Intel UHD Graphics 620 |
| SSD | 2TB WD SN5000 |
| WiFi & BT | Intel AX201 |
| SMBIOS | MacBookPro 16,3 |
| MacOS | MacOS Sequoia


## Current Bugs
1. The display brightness will be extremely dimm for the first 140-180 seconds after entering the desktop environment.
2. The trackpad doesn't work to wake from sleep, but Enter/Space work.
3. Gesture Controls do not work with the trackpad, this can be quite annoying on other laptops, but the latitude has 2 sets of right and left click buttons.
4. Battery seems to drain faster than using Mint/Windows?
