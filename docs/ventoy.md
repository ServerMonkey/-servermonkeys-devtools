# Ventoy with Debian Preseed and fastpkg

This guide will show you how to create a USB-installation stick, for
automated installation of Debian with Ventoy and a Preseed file. It will also
show you how to use fastpkg to download the necessary files faster.

## Automatic installation, with fastpkg

THIS SECTION IS NOT FINISHED  
Ask me in chat or via mail.

This will use my own generic template files.  
This requires that you already have installed fastpkg and added a fastpkg
repository that includes the files below. If not follow this guide:
[github.com/ServerMonkey/fastpkg](https://github.com/ServerMonkey/fastpkg)

Open a terminal and run:

`sudo fastpkg -p ventoy install`

`sudo fastpkg -p "debian-11-firmware-dvd1 servermonkeys-templates" download`

## Manual installation, without fastpkg

Download and install Ventoy  
https://www.ventoy.net/en/download.html

Download a Debian 11 ISO  
https://cdimage.debian.org/cdimage/unofficial/non-free/cd-including-firmware/archive/

Download a Debian Pressed file.  
The latest example version can be downloaded here:  
https://www.debian.org/releases/stable/example-preseed.txt

Or check Archive.org for older versions (check your Debian release):  
https://web.archive.org/web/*/https://www.debian.org/releases/stable/example-preseed.txt

Modify the Pressed file to your liking and include it in Ventoy.  
To understand how to modify the Pressed file, read this manual:  
https://wiki.debian.org/DebianInstaller/Preseed  
To understand how to include the Pressed file in Ventoy, read this manual:  
https://www.ventoy.net/en/plugin_autoinstall.html
