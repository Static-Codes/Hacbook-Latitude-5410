# Notes:
This is **not a plug and play solution** for you to run MacOS Sequoia on your Dell Latitude 5410.

**This configuration is currently semi functional, the operating system works, but it has a few significant bugs/unpatched features**.

Please **do not** use this repository for **anything** other than **occasional references**; for **ALL** questions, please refer to *[Dortania's Guide on Open Core](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/)*

Since this I'm triple booting on the same SSD, I have chose not to add macOS to my internal EFI partition, instead opting to keep an SD card with the bootloader inside the laptop; This is completely unnecessary for users not intended to dual or triple boot with Windows and MacOS.

## Laptop Specs – Latitude 5410 (P98G007)

| Component            | Specification                                                                |
| ----------------- | ------------------------------------------------------------------ |
| CPU | i5-10210U  |
| iGPU | Intel UHD Graphics 620 |
| SSD | 2TB WD SN5000 |
| WiFi & BT | Intel AX201 |
| SMBIOS | MacBookPro 16,3 |
| MacOS | MacOS Sequoia

## Triple Boot Setup
| OS              | Partition Size | Partition Order |
| :---:           | :---:          | :---:           | 
| Debian 13       | 810 GB         | 1               |
| MacOS (Sequoia) | 800 GB         | 2               |
| Win11 (LTSC)    | 200 GB         | 3               | 

## Current Bugs
1. The trackpad doesn't work to wake from sleep, but Enter/Space work.
2. Gesture Controls do not work with the trackpad, this can be quite annoying on other laptops, but the latitude has 2 sets of right and left click buttons.
3. There is no patch in this config for backlight initialization. Currently, it takes around 3-5 minutes for the display to reach its intended brightness.

## Notes:
1. The battery seems to discharge faster than using Linux/Windows, I haven't ran Power Management tests yet though. 
