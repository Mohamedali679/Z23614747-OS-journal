# Week 1 – System Planning and Setting Up the Project

This week I mainly focused on planning how my whole setup is going to work. Before doing any real server configuration, I needed to decide what systems I am using, how they connect to each other, and why I chose them.
---

## System Architecture

I decided to use my HP Windows laptop as the workstation. This will be the machine I use to connect to the server using SSH.  
The server itself will be an Ubuntu Server 22.04 LTS virtual machine running in VirtualBox. The server will be headless, meaning no graphical interface is installed, and all administration will be done through the command line.

The basic setup looks like this:

Windows Laptop (Workstation)
|
| SSH connection
|
Ubuntu Server 22.04 LTS (VirtualBox VM)
