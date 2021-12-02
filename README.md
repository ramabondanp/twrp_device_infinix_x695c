# TWRP device tree for Infinix Note 10 Pro ID (X695C)

## Status

Current state of features (from [here](https://twrp.me/faq/OfficialMaintainer.html)):

### Blocking checks

- [ ] Correct screen/recovery size
- [ ] Working Touch, screen
- [ ] Backup to internal/microSD
- [ ] Restore from internal/microSD
- [ ] reboot to system
- [ ] ADB

### Medium checks

- [ ] update.zip sideload
- [ ] UI colors (red/blue inversions)
- [ ] Screen goes off and on
- [ ] F2FS/EXT4 Support, exFAT/NTFS where supported
- [ ] all important partitions listed in mount/backup lists
- [ ] backup/restore to/from external (USB-OTG) storage (not supported by the device) (not tested)
- [ ] [backup/restore to/from adb](https://gerrit.omnirom.org/#/c/15943/)
- [ ] decrypt /data
- [ ] Correct date

### Minor checks

- [ ] MTP export
- [ ] reboot to bootloader
- [ ] reboot to recovery
- [ ] poweroff
- [ ] battery level
- [ ] temperature
- [ ] input devices via USB (USB-OTG) - keyboard, mouse and disks (not supported by the device) (not tested)
- [ ] USB mass storage export (not tested)
- [ ] set brightness
- [ ] vibrate (Doesn't work, WIP)
- [ ] screenshot
- [ ] partition SD card

## Building

```bash
source build/envsetup.sh
lunch twrp_x695c-eng
mka bootimage
```

