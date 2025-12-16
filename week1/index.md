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
---

## Distribution Choice – Ubuntu Server 22.04 LTS

I chose Ubuntu Server 22.04 LTS for the server operating system for a few reasons.

Firstly, Ubuntu Server is very well documented, which makes it easier to learn and troubleshoot when setting up services like SSH, firewalls, and security tools.  
Secondly, the LTS (Long Term Support) version is stable and receives security updates for several years, which makes it suitable for a secure server environment.

Ubuntu Server is also lightweight because it installs without a desktop environment by default. This is useful for performance testing later in the coursework and matches the requirement for a headless server.  
Another reason is that Ubuntu uses AppArmor by default, which will be useful later when implementing mandatory access control.
---

## Workstation Choice

For the workstation, I am using my Windows laptop instead of setting up a second Linux virtual machine.

I chose this because running only one VM reduces the load on my laptop and makes the system more stable. Windows also has built-in SSH support through PowerShell and Windows Terminal, so I can connect to the server without installing extra tools.

This setup also reflects real-world scenarios, where Linux servers are often managed remotely from Windows machines.
---

## Planned Network Configuration

The virtual machine will be configured with two network adapters in VirtualBox:

- **NAT adapter** – This will allow the server to access the internet for updates and package installation.
- **Host-only adapter** – This will create a private network between the Windows workstation and the Ubuntu server, allowing SSH access.

The host-only network usually uses an IP range such as `192.168.56.0/24`.  
Once the server is installed, I will find its IP address using the `ip addr` command and use that address to connect via SSH.
---

## Planned System Information Commands

After installing Ubuntu Server, I will run the following commands over SSH to document the system details:

uname -a
free -h
df -h
ip addr
lsb_release -a

These commands will show information about the kernel, memory usage, disk usage, network interfaces, and the installed Ubuntu version. This information will be useful later when analysing performance and system behaviour.
---

## Reflection

This week was mainly about planning rather than implementation. Choosing a simple setup with one server VM and a Windows workstation makes the system easier to manage and follows the coursework rules closely.

Understanding how the server and workstation interact through SSH is important before moving on to security configuration and performance testing in the next weeks.
