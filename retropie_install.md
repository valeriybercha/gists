# Install and set-up Retropie on Raspberry Pi 4 model B

Pre-requisites:
- Raspberry Pi microcomputer (4 model B 2Gb in my case)
- Micro SD card (64 Gb memory in my case)
- Gamepad
- HDMI cable to connect the Raspberry Pi to monitor

### Install 'Retropie' operating system

1. Download and install Raspberry Pi Imager from the official website - https://downloads.raspberrypi.org/imager/imager_1.5.exe
2. Plug in the Micro SD into your computer.
3. Open the Raspberry Pi Imager.
4. Click on 'CHOOSE OS' button and select 'Reropie' operating system.
5. Select the correct version for your Raspberry Pi model (ex: RetroPie 4.6(RPi4)).
6. Click on 'CHOOSE SD CARD' button and choose the Micro SD card you inserted earlier.
7. Click on 'WRITE' button. 'Retropie' system will be installed on your SD card.
8. Eject the Micro SD card and insert it into your Raspberry Pi device. Plug-in also the game controller into the Raspberry Pi.
9. Power on the Raspberry Pi and wait for game controller to be detected.
10. Configure your controller.

### Connect the device to the internet

11. Eject the micro SD from the Raspberry Pi and insert it into the computer.
12. Open the default directory of the micro SD card.
13. Create 'wifikeyfile.txt' file in the root directory
14. Open the created file with a text redactor and type the following lines:
```sh
ssid="Your Wi-fi netword ssid"
psk="Your wi-fi network password"
```
Save the changes.

15. Eject the micro sd card from the computer and insert it back again into Raspberry Pi.
16. Turn on the Raspberry, select the Retropie configuration. From the menu select 'WIFI'.
17. From the opened window select the 'Import WiFi credentials from /boot/wifikeyfile.txt'. Click 'OK' button.
18. The system will be connected to wi-fi and you will receive an IP address(ex: Current IP: 192.168.0.101). Remember this IP address.

### Expand filesystem partition
19. From the 'Retropie' configuration menu select 'RASPI-CONFIG'. From the opened indow select 'Advanced options'. Then select 'Expand Filesystem'.
The system memory will be expanded to your micro SD card memory.

### Installing custom ROM's

20. Go to your computer and in the computer folder type ```\\192.168.0.101``` (IP address from your Retropie connected ti the internet).
21. A new folder 'roms' should appear. If you receive an error message,it means that Windows cannot connect to network computer (Open 'Registry Editor' in Windows -> 'HKEY_LOCAL_MACHINES' -> 'SYSTEM' -> 'CurrentControlSet' -> 'Services' -> 'LanmanWorksation' -> 'Parameters' -> 'AllowInsecureGuestAuth' and set the 'Value data' parameter to '1').
22. Open the 'roms' folder and copy roms to the corresponded game platform folder.
23. Restart the 'EmulationStation' on Raspberry Pi (click on 'Start' button on controller -> select 'QUIT' option -> 'RESTART EMULATIONSTATION').

### Installing custom ROM's for 'Dreamcast' platform

24. Folder for Dreamcast platform is not created by default. You have to create 'dreamcast' folder in 'roms' directory.
25. Copy a dreamcast rom in the created 'dreamcast' directory.
26. You also need to install the emulator for Dreamcast platform to play the games. For this go to: 'Retropie configuration' -> 'Retropie setup' -> 'Manager packages' -> 'Manage experimental packages' -> and choose 'redream' emulator.
27. Restart the 'EmulationStation' on Raspberry Pi (click on 'Start' button on controller -> select 'QUIT' option -> 'RESTART EMULATIONSTATION').