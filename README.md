# Dual-booting with Ubuntu and Windows

## Introduction
This guide will walk you through the process of installing Ubuntu alongside your Windows operating system on your computer. 

#### Notes:
* For Mac users, follow this [documentation](https://help.ubuntu.com/community/DualBoot/MacOSX).
* Understand that partitioning your hard drive comes with the risk of losing data on your computer.

## Required materials
* A flash drive with a capacity of at least 2GB. Make sure that there are no important files on it because they will be erased during this process.
* A computer that can boot (start-up) from a USB memory stick. Many older computers can't boot from USB so check the boot options in your BIOS to see if yours can.
* A computer with:
  * at least 2GB of memory (RAM)
  * 6GB of available hard disk space
* Internet connection

## 1. Preparation  
* If you are afraid of losing files on your computer, make sure to [back up your data](https://help.ubuntu.com/community/BackupYourSystem) before attempting a dual-boot installation. 
* It is also a good idea to have a [Windows recovery CD/DVD](https://help.ubuntu.com/community/WindowsRecoveryCd) available.
* Check how many GB of hard disk space you have available.

## 2. Create a Bootable USB Memory Stick
You will use a USB memory stick with a copy of the Ubuntu installer CD image (.iso) to install Ubuntu. If you already have one, skip this step.

### Get a Copy of Ubuntu Installer
To install Ubuntu, you need to download copy of the Ubuntu installer CD image (.iso).
1. Go to http://www.ubuntu.com/getubuntu/download
2. Download the latest version of Ubuntu. In this case, Ubuntu 16.04.2 LTS.

### Put Ubuntu Installer on USB Memory Stick
You need to download a program that can properly put the installer onto a memory stick. You can't just copy the .iso file onto the memory stick.
1. Plug-in your USB memory stick.
2. Go to https://rufus.akeo.ie/ and download the Rufus USB installer.
3. See the detailed instructions at the Rufus website or at https://www.ubuntu.com/download/desktop/create-a-usb-stick-on-windows.

## 3. Start the Ubuntu Installer
1. Plug-in your USB memory stick and restart your computer.
2. As soon as you see text on the screen, hit F12 to open the BIOS setup.
    * If F12 doesn't work, you might have to hit one of these keys instead: F1, F2, Del, Esc, F10, F11.
3. A BIOS screen should appear. Find the option to change the Boot Order and change the first item in the boot order list to be your USB memory stick.
4. After changing the boot order, save your changes and restart your computer. It should now start from the USB memory stick.

## 4. Install Ubuntu
1. After restarting your computer and starting to boot from the USB memory stick, an install window should appear. Pick "Install Ubuntu".
2. Follow the instructions on the screen to select your country, time zone and keyboard layout.
3. When you get to the Partitioning screen, choose Install Ubuntu alongside Windows. 
    * This is called a dual-boot setup. 
4. Use the slider in the next window to choose how to share disk space between Windows and Ubuntu. 
    * Ubuntu should have at least 8 GB of space. It works better with 16 GB or more, which should be possible in a not too old computer.
    * Make sure you leave enough room for your Windows operating system.
5. When you click Forward, you may receive a message saying that the changes will be applied. This normally happens if you resized a partition. If you click Continue, your hard disk will be changed permanently and you won't be able to go back. Make sure you're happy with any changes that you made.
6. Follow the rest of the instructions to choose a username and password and migrate files and settings from Windows.
   * The username and password you choose will be needed to log on to your computer.
7. Click Install. The installation will begin, and should take 10-20 minutes to complete. 
8. When it is finished, choose to restart the computer and then remove your memory stick. Ubuntu should start to load.
