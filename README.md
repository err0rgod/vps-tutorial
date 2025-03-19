# vps-tutorial
This repository is to help with building your own vps from using your old pc hardware.

## Required Components.

1. PC Hardware which is working display, keyboard, maouse doesn't matter.
2. External temporary Moniter for setting up OS. (can use a tv)
3. Storage as you Required.
4. Wifi Connection. as we need to enable port forwarding to publish it on WAN.
5. Bootable pendrive minimum 8 gb.
6. Guts to face errors.
7. Follow to err0rgod.

## OS Installation

First we need to Install The Operating System, I prefer Kali Linux as it is pretty easy to work on. First we need to install the operating system from [Kali.org](https://www.kali.org/get-kali/#kali-installer-images) then we need to flash it to the Bootable pendrive. to flash it we need to download ventoy from [ventoy](https://sourceforge.net/projects/ventoy/files/v1.1.05) then after downloading it open ventoy2disk.exe and select the pendrive you want to boot then click on Install Button after this you just need to paste the iso file into the bootable pendrive and your work is done. Now you Just need to Install the OS on laptop you just need to plug the pendrive and install it. It is a quite easy process for any confuse watch the kali installation video on my channel or you can directly contact me.

## Cnfigure SSH

This is the main process as in this process we need to Configure Our machine to run ssh service.

First you need to insstall OPENSSH

``` bash 
sudo apt update & sudo apt install -y openssh-server
```

Start The SSH Service 

``` bash
sudo systemctl start ssh
sudo systemctl enable ssh
```
Check the ssh status 

``` bash
sudo syetemctl status ssh
```

Now we are done configuring SSH.

## Connecting on LAN

To connect to it you need to you need to get the local ip of the kali linux by running command.
``` bash
ifconfig
```

after that try to connet to it from another computer connected on the same network by cmd or shell

``` bash
ssh kali-user@ip-of-linux-machine
```
Now you will be connected to the shell of the kali linux by ssh.

## Configure For Public Access over WAN.

Now you have to play with the Router and some advance stuff for proceeding further so i will recommend you to watch the video properly and if you have any doubts you can directly DM me [message me](https://instagram.com/err0rgod)
