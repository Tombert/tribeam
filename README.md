# Welcome  
This script will create a hackintosh USB-installer with the latest github release of OpenCore bootloader,  
it uses the Basesystem.dmg of the macOS app which is a net-installer and download the  
necessary packages during installation there for you need internet connection to use it.    
## Getting Started
You'll need Ubuntu, Arch, Fedora , or Debian based distros for it to work any other distro aren't supported for now.

## Step 1
Plug in your USB-drive 4GB or more. 

## Step 2
Run `tribeam.sh` to download installation media for macOS (internet required)   
Select the macOS version desired:


## Step 3
Select the USB-drive whenever the script asks, it will show a menu with all drives For example:
```
1) sda 500GB
2) sdb 16GB
#)?
```

in this example 2 is the usb drive so typpe 2 and press enter.
be carefull not to select your ssd as it would wipe it clean.

## Step 4
Wait for the instalation to finish, open ``/mnt`` and edit your config.plist with ProperTree:  
https://github.com/corpnewt/ProperTree  
You may have to change the python path of ``ProperTree.command``  
from ``#!/usr/bin/env python``
to ``#!/usr/bin/env python3`` and install ``python3-tk`` for it to work  
eg for ubuntu ``sudo apt install python3-tk`` then,  
Fallow the OpenCore Vanilla guide:  
https://dortania.github.io/OpenCore-Desktop-Guide/    
***Credits to: IgorBressan for  <a href="https://github.com/IgorBressan/macOSDownloader" target="_top">macOSDownloader</a>***


