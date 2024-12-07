# PiNAS

This project showcases a Network-Attached Storage (NAS) system built using a Raspberry Pi 4 running Debian Linux Sandworm 7.4.15-2. The system is powered by OpenMediaVault for easy configuration and management, designed to operate as a secure and efficient file storage solution on a local area network (LAN). Based on <a href ="https://youtu.be/gyMpI8csWis?si=il20hzJr9_SuEvVr">Networkchuck's YouTube video tutorial of the same subject </a>

# Main features

-Accessible file storage through a network share utilizing SMB service<br>
-User friendly administration with openmediavault<br>
-Integrated disk management<br>
-Support for multiple file sharing protocols (SMB, CIFS and NFS)<br>

# Hardware

-A computer with internet connection
-Raspberry Pi 4 model B 8GB with power supply<br>
-Raspberry Pi case (optional)<br>
-MicroSD card<br>
-Memory card reader<br>
-External strorage (Kingston Datatraveler 3.0 128GB used in this case)<br>
-Switch/router/modem with Ethernet connection<br>
-Ethernet cable cable<br>

# Software

-Raspberry Pi Imager<br>
-Raspberry OS Lite (64bit)<br>
-openmediavault NAS solution<br>
-openmediavault installation script:<br> 

# Network setup

-LAN with static IP configuration preferred<br>

#Installation (Raspberry Pi OS to memory card)

-Download and install <a href="https://www.raspberrypi.com/software/">Raspberry Pi Imager<a><br>
-Insert the SD card to the SD card reader and run Raspberry Pi Imager<br>
-Select your Raspberry Pi device (Raspberry Pi 4), OS (Raspberry Pi OS (other) -> Raspberry Pi OS Lite (64bit))<br>
-Select your storage media **(make sure to select the SD card!)**<br>
-Press ctrl+shift+X for OS customization.<br>
-From general tab set your hostname, username and password and enable SSH<br> This enables headless use and the option to access the computer remotely.<br>
-From services tab enable SSH and select to use password authentication<br>
-Select "Save"<br>
-After configuring these options select WRITE and YES at the Raspberry Pi Imager, the OS will install now.<br>
-Insert the SD card to Raspberry Pi and connect ethernet and power supply cables.

#Installation (openmediavault to Raspberry Pi)

-Open cmd/terminal and connect to your Raspberry Pi via SSH:<br>
-`ssh <yourpiname>@xxx.xxx.xxx.xxx` <- your Pi's IP address. Check the IP address from your home router. The following prompt appears:<br>
-![image](https://github.com/user-attachments/assets/9fa86a1a-32ca-4d89-b0bf-bb4e2e736dc1) type in yes to continue.<br>
-Once logged in, update your Pi:<br>
-`sudo apt update && sudo apt upgrade`<br>
-After the update install openmediavault:<br>
-`wget -O - https://raw.githubusercontent.com/OpenMediaVault-Plugin-Developers/installScript/master/install | sudo bash`

#Configuring openmediavault

#Disclaimer:

-All content in this repository is for author's study and documentation practice purposes only.
-Contents of this repository is not to be used in production or education
-This repository is not to be referred as a valid source in production or educational environments.
-All referenced content belong to their rightful owners












