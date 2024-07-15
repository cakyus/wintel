# Wintel

Purpose: enable WSL to rule them all.

![Wintel 0](Pictures/wintel-0.jpg)

## Hardware Specification

 1. CPU: Intel Cherry Trail CR Atom Z8350
 2. Memory: RAM 4GB ROM 64GB
 3. OS: Windows 10 Pre-installed
 4. Network: RJ45 100M, WiFi 802.11 2.4G+5.8G, Bluetooth 4.2
 5. USB: USB 3.0
 6. Accessories: Power Adapter, HDMI Cable, User Manual.

## TIPS

 1. Use cmd.exe, do not use mintty, charset is broken.

## Installation

 1. Install Windows OpenSSH
 2. Install Windows Subsystem for Linux

### Setup vim

    sudo apt remove nano
    sudo apt install vim

Fix vim start in replace mode. https://superuser.com/a/1525060

    ~/.vimrc
    set t_u7=

### Setup cron (Work In Progress)

    /etc/wsl.conf
    [boot]
    command="service cron start"

### Setup PHP

All scripts will be written in PHP.

    sudo apt install php-cli

## Resources

 1. https://github.com/microsoft/WSL/

## TODO

 * Login OpenSSH using private key
 * Auto login SSH to WSL
 * Wifi auto connect script
 * Resource monitor
 * Restart server in WSL
