### Linux Environment Setup Using Ubuntu and VirtualBox

## Project Overview

This project demonstrates how to set up a Linux environment from scratch using Ubuntu inside a virtual machine. The setup uses Oracle VM VirtualBox to run Ubuntu safely on a host operating system without affecting the host machine.

This guide documents the full process including downloading software, creating a virtual machine, installing Ubuntu, and verifying the system.

-------------------------------------------------------------------------------

## Technologies Used

| Tool                 | Description                                        |
| -------------------- | -------------------------------------------------- |
| Ubuntu 22.04 LTS     | Linux operating system used in the virtual machine |
| Oracle VM VirtualBox | Virtualization software used to run Ubuntu         |
| Windows              | Host operating system                              |

-------------------------------------------------------------------------------

## System Architecture

Host Machine (Windows)
↓
VirtualBox Hypervisor
↓
Ubuntu Virtual Machine

This setup allows Ubuntu to run as a separate system inside the host machine.

------------------------------------------------------------------------------

## Step 1 — Download Required Software

Download Ubuntu Desktop ISO.

Example file:

```
ubuntu-22.04.5-desktop-amd64.iso
```

Download and install VirtualBox for your system.

------------------------------------------------------

## Step 2 — Create a Virtual Machine

Open VirtualBox and click **New**.

Configure the virtual machine with the following settings:

Name:

Ubuntu

Type:

Linux

Version:

Ubuntu (64-bit)

------------------------------------------------------

## Step 3 — Allocate System Resources

Assign system resources to the virtual machine.

RAM:

4096 MB

CPU:

2 processors

------------------------------------------------------

## Step 4 — Create Virtual Hard Disk

Disk Type:

VDI (VirtualBox Disk Image)

Storage Type:

Dynamically Allocated

Disk Size:

40 GB

---------------------------------------------------------

## Step 5 — Attach Ubuntu ISO

1. Open VM Settings
2. Navigate to Storage
3. Under Controller IDE select **Empty**
4. Attach the Ubuntu ISO file

----------------------------------------------------------

## Step 6 — Boot the Virtual Machine

Start the VM.

Ubuntu boot menu will appear.

Select:

Try or Install Ubuntu

----------------------------------------------------------

## Step 7 — Install Ubuntu

Select the following options during installation.

Language:

English

Keyboard Layout:

English (US)

Installation Type:

Normal Installation

Enable:

Download updates while installing
Install third-party software

------------------------------------------------------------

## Step 8 — Disk Configuration

Choose:

Erase disk and install Ubuntu

Note: This affects only the virtual disk created inside VirtualBox.

----------------------------------------------------------------

## Step 9 — Create User Account

Example configuration:

Name: Student

Computer Name: ubuntu-vm

Username: student

Password: ********

-----------------------------------------------------------------

## Step 10 — Complete Installation

Ubuntu installs the system files.

Installation time:

5–10 minutes

After installation click:

Restart Now

------------------------------------------------------------------

## Ubuntu Desktop Environment

After restarting, Ubuntu will load the desktop environment successfully.

---

## Verify Installation Using Terminal

Open Terminal and run:

```
pwd
ls
uname -a
sudo apt update
```

These commands confirm the Linux environment is working correctly.

----------------------------------------------------------------------

## Project Outcome

Successfully created a Linux environment using Ubuntu and VirtualBox.

This setup provides a safe environment for:

* Learning Linux commands
* Development work
* Cybersecurity practice
* System administration training

------------------------------------------------------------------------

## Future Improvements

Possible enhancements for this setup:

* Install VirtualBox Guest Additions
* Enable shared folders between host and VM
* Install development tools
* Configure networking

