# arkos4clones – Linux Guide

A guide for setting up **arkos4clone** on Linux.

---

## 1. Download & extract the image

- Download **all four compressed archives** from the latest [arkos4clone release](https://github.com/lcdyk0517/arkos4clone/releases)
- Install **7-Zip** for your distribution (example for Arch Linux):
```bash
sudo pacman -S 7zip
```
(You need 7-Zip because some default file managers may fail to extract the archive correctly)
- Go to your download directory and extract the first archive part, which should automatically extract all four parts into one zip file:
```bash
7z x ArkOS4Clone-20251213.zip.7z.001
```
_(Replace the filename with the first part of your downloaded archive, the version shown here may already be outdated)_
- After extraction, you should have a .zip file. Extract it:
```bash
7z x ArkOS4Clone-20251213.zip
```
_(Use the password from the release page.)_
- You should now have a .img file

## 2. Flash the image to your new SD card

- Flash the .img file to your SD card using [Balena Etcher](https://etcher.balena.io/#download-etcher)
  - Select the .img file
  - Select your SD card
  - Click Flash
- _You should disable “Trim unallocated space on raw images (in ext-type partitions)” in settings, as it may cause issues._
- Please refer to the [Handheld Wiki Recommendations](https://handhelds.wiki/R36S_Compatibility_Lists#SD_Cards) when buying a SD card, as some may not work)

## 3. DTB Selection
- If you dont have the .dtb filese because your R36S clone has the original OS stored internally (not on the SD card), like mine did, manually add the files to your SD card like instructed in the [official readme](https://github.com/lcdyk0517/arkos4clone?tab=readme-ov-file#how-to-use), as the dtb-selector tool is only available for mac and windows, as of writing this guide.

## 4. First Boot
- If you see a Boot Logo ArkOS is working, the first start will take a while as its creating lots of directories and also a EASYROMS Partition where you can put your game roms afterwards.
- If you dont know where to get your ROMs from, check the [r/ROMS Wiki](https://www.reddit.com/r/Roms/wiki/index/) :)

**Have fun :)**



