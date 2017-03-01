# mac_iso_usb

## Description how to make a bootable usb from an iso on mac1. download the iso
2. convert iso to 
	hdutil convert -format UDRW -o ./ubuntu-14.04.3-server-amd64.img ./ubuntu-14.04.3-server-amd64.iso3. diskutil list
4. put in the usb
5. diskutil list , and find the new disk
6. diskutil unmountDisk /dev/disk3    // if it's on disk3
7. dd if=/Users/tschoots/Downloads/ubuntu/ubuntu-16.10-desktop-amd64.img.dmg of=/dev/disk3 bs=1m
8. diskutil eject /dev/disk3