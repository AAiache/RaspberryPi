# RaspberryPi
## 1. Set up the SD Card

####Download the Hypriot Docker SD card image:  
   http://blog.hypriot.com/downloads/  
Because you will need an SD-card with a bootable linux image.  
####Flash the downloaded image to your SD card: 
-unzip the downloaded image first!  
-Put your SD Card into your Mac  
-Run:  

    diskutil list
-Get the identifier of the SD Card (/dev/diskxx)
-Unmount the SD card:  

    diskutil unmountdisk /dev/diskxx
-Flash your SD Card:  

      sudo dd if=hypriot-rpi-201???.img of=/dev/rdiskxx bs=1m  

## 2. Share internet Connection with you Pi

- Plugin  your Pi to your MAc using an ethernet cable
- Open System Preferneces / Sharing 
- Ckeck the "Internet Sharing" case.

## 3. Connect to your Raspberry Pi via ssh:

    arp -a
Get the IP address of the raspberry Pi

    ssh pi@xx.xx.xx.xx
# Have fun!
