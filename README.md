# coreboot-config
All the nessecary files for Corebooting a Thinkpad T440p. 
# Preface
* All blobs are board specific so for each device you will need to take your own readings using a 3.3V CH341A SPI Flasher  
* This guide is mainly meant to serve a reference material should I need to do this process again at a later date. This should serve to assist you if any errors occur and should serve to further your understanding of the process of Corebooting the Thinkpad T440p is it not meant to be a all encompassing tutorial
* I am working off the tutorial kindly provided at https://blog.0xcb.dev/lenovo-t440p-coreboot/, I have of course made some modifications to suite my own needs however my process still rather strictly adhere's to the guide and as such if you intend of using the repo for your own purposes I would recommend also reading through the link provided.

# Requirements
Commands for installing the nessecary requirements are listed here
## Debian 11(Recommended)
sudo apt install libncurses-dev build-essential curl nasm sharutils unzip zlib1g-dev m4 bison flex gnat uuid-dev python
## Arch
sudo pacman -S base-devel curl git gcc-ada ncurses zlib nasm sharutils unzip flashrom python3
Please note this will fail to compile with anything other than GCC10. I recommend using Debian 11 as GCC10 is the default cross compilier

# Installation
Follow the guide [here](https://blog.0xcb.dev/lenovo-t440p-coreboot/ 'Lenovo T440p Coreboot') 

Populate .config through running make nconfig, savings through F6 and then quitting through F9
