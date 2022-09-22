# coreboot-config
All the nessecary files for Corebooting a Thinkpad t440p.

Requirements
sudo apt install libncurses-dev build-essential curl nasm sharutils unzip zlib1g-dev m4 bison flex 
Please note this will fail to compile with anything other than GCC10. I recommend using Debian 11 as GCC10 is the default cross compilier

Installation
Clone the repository

Populate .config through running make nconfig, savings through F6 and then quitting through F9
