# PiNAS

This project showcases a Network-Attached Storage (NAS) system built using a Raspberry Pi 4 running Debian Linux Sandworm 7.4.15-2. The system is powered by <a href="https://www.openmediavault.org">openmediavault</a> for easy configuration and management, designed to operate as a secure and efficient file storage solution on a local area network. Inspired by <a href ="https://youtu.be/gyMpI8csWis?si=il20hzJr9_SuEvVr">Networkchuck's YouTube video on the same subject </a>

## Features

* Accessible file storage through a network share utilizing SMB service
* User friendly administration with openmediavault
* Integrated disk management
* Support for multiple file sharing protocols (SMB, CIFS and NFS)

## Prerequisites

* General knowledge of Windows, Linux, computer hardware and networking

## Hardware requirements

* A computer with internet connection
* Raspberry Pi 4 model B 8GB with power supply
* Raspberry Pi case (optional)
* MicroSD card
* Memory card reader
* External strorage (Kingston Datatraveler 3.0 128GB used in this case)
* Switch/router/modem with Ethernet connection
* Ethernet cable cable

## Software requirements

* Raspberry Pi Imager
* Raspberry OS Lite (64bit)
* openmediavault NAS solution

## Network requirements

* Internet connection
* Static IP configuration is recommended for stable access.

## Installation (Raspberry Pi OS to memory card)

* Download and install <a href="https://www.raspberrypi.com/software/">Raspberry Pi Imager<a>
* Insert the SD card to the SD card reader and run Raspberry Pi Imager
* Configure the following:
  *  (Raspberry Pi 4)
  *  OS (Raspberry Pi OS (other) -> Raspberry Pi OS Lite (64bit))
  * Select your storage media **(make sure to select the SD card!)**
* Press ctrl+shift+X for OS for advanced settings.
  * **General**: Set your hostname, username and password and enable SSH for remote access
  * **Services**: Enable SSH with password authentication
* Select "Save"
* After configuring these options select WRITE and YES at the Raspberry Pi Imager, the OS will install now.
* Insert the SD card to Raspberry Pi and connect ethernet and power supply cables.

## Installation (openmediavault to Raspberry Pi)

* Open a terminal and SSH to your Raspberry Pi:
* `ssh <your_username>@xxx.xxx.xxx.xxx` <- your Pi's IP address. Check the IP address from your home router. The following prompt appears:
* ![image](https://github.com/user-attachments/assets/9fa86a1a-32ca-4d89-b0bf-bb4e2e736dc1)
* Type in yes to continue.
* Once logged in, update your Pi:
* `sudo apt update && sudo apt upgrade`
* After the update run the script below to install openmediavault:
* `wget -O - https://raw.githubusercontent.com/OpenMediaVault-Plugin-Developers/installScript/master/install | sudo bash`

## Configuring openmediavault

WIP

## Configuring network share on Windows 11

WIP

## Sources:

* <a href="https://www.openmediavault.org">Openmediavault</a>
* <a href="https://academy.networkchuck.com">Networkchuck</a>

## **Disclaimer:**

* All content in this repository is for author's study and documentation purposes only.
* The contents are not intended for production or educational use.
* Always verify sources and review scripts before running them.
* All referenced content belong to their rightful owners.
