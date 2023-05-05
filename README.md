# unraid_vm_icons

This is a fork of [SpaceinvaderOne](https://github.com/SpaceinvaderOne/unraid_vm_icons)s excellent Docker Container for adding VM icons to the Unraid VM Manager.  

I wanted to go with a different approach, as I want as little as possible clutter among my containers.

All the icons have been compiled into a Slackware Package, that unRaid can install on boot.  
This will install all the included icons, but not touch the original ones.  

### Installing
To install the icons, grab the latest .txz-file from the [releases](https://github.com/Lanjelin/unraid_vm_icons/releases/), and store it somewhere on your server.  
Open a terminal, and navigate to the file, then run `installpkg unraid_vm_icons.txz`, and you should recieve a promt that the contents have been installed.  
To make the icons install on boot, move the .txz-file to the extra-folder on the flash drive; `mv unraid_vm_icons.txz /boot/extra`  

### Uninstalling
Should you wish to uninstall the icons, remove the file from /boot/extra, take note of it's exact name,
then run eg. `removepkg unraid_vm_icons-2023.05.05-x86_64-1_lanjelin` (without the file extension).

### Updating
Follow the instructions for Uninstalling, then Installing.
