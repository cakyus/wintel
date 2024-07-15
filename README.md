# Wintel

Purpose: manage everything in Mini PC using WSL.

## Hardware Specification

 1. CPU: Intel Cherry Trail CR Atom Z8350
 2. Memory: RAM 4GB ROM 64GB
 3. OS: Windows 10 Pre-installed
 4. Network: RJ45 100M, WiFi 802.11 2.4G+5.8G, Bluetooth 4.2
 5. USB: USB 3.0
 6. Accessories: Power Adapter, HDMI Cable, User Manual.

## TIPS

 1. Do not use mintty, charset is broken.

## Installation

 1. Install Windows OpenSSH
 2. Install Windows Subsystem for Linux

### Setup vim

    sudo apt-get remove nano
    sudo apt-get install vim

Fix vim start in replace mode. https://superuser.com/a/1525060

    ~/.vimrc
    set t_u7=

### Setup cron

    /etc/wsl.conf
    [boot]
    command="service cron start"

## TODO

 * Login OpenSSH using private key
 * Auto login SSH to WSL
 * Wifi auto connect script
 * Resource monitor
 * Restart server in WSL
