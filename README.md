## What is operating system ?
#### An opearting system is a system software that manages system software and hardware resources.
#### It is act as intermidiate between user and the hardware.
#### Os manages the Hardware resource and provide services for computer program .
### Main Functions of an Operating System
1) User Interface – Provides GUI or Command Line
2) Process Management – Runs multiple programs at the same time
3) Memory Management – Allocates and frees RAM
4) File System Management – Organizes files & folders
5) Device Management – Controls keyboard, mouse, printer, etc.
6) Security & Access Control – Protects data and users


# linux
#### Linux is a operating system that manages the computer hardware and software resource .It act as a intermediate between user and the hardware. linux is a open source operating system based on unix.linux is a kernel. linux uses command line interface.


# linux architecture 
<img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/984e84ac-73df-415f-9d8f-87cd4b552037" />

### 1) Hardware
#### hardware is a physical component of the computer system .it consist of motherboard ,cpu, hdd, ram etc
### 2) Kernel
#### - Kernal is a core part of the linux . <br> - kernal is a heart of the linux <br> - kernal is a bridge between software and hardware of computer .<br> - kernel manages the system resources <br> - linux kernel is a free and open source.

### 3) Shell
#### shell can provide interface to user to communicate with the kernel <br> - it is a interface to interact with os using command .

### 4) Application
#### it is a tool and software to perform tasks. user interact with the system through various application such as office and games etc.

# 19 directories in linux 

# 📁 Linux Directory Structure (19 Important Directories)

| Directory | One-Line Explanation |
|----------|----------------------|
| `/` | Root directory — starting point of the entire Linux file system. |
| `/bin` | Essential user command binaries (ls, cp, mv, cat). |
| `/boot` | Boot loader files and Linux kernel images. |
| `/dev` | Device files representing hardware components. |
| `/etc` | System-wide configuration files. |
| `/home` | Home directories of normal users. |
| `/lib` | Shared libraries required by system binaries. |
| `/media` | Mount point for removable media (USB, CD). |
| `/mnt` | Temporary mount point for filesystems. |
| `/opt` | Optional third-party application packages. |
| `/proc` | Virtual filesystem providing process and kernel info. |
| `/root` | Home directory of the root (admin) user. |
| `/run` | Runtime data like PID files and sockets. |
| `/sbin` | System administration binaries (reboot, fsck). |
| `/srv` | Data for services like web or FTP servers. |
| `/sys` | Virtual filesystem exposing kernel devices and drivers. |
| `/tmp` | Temporary files (cleared on reboot). |
| `/usr` | User applications and utilities. |
| `/var` | Variable data like logs, mail, cache, spool files. |

---

### ⭐ Interview One-Line Summary

Linux uses a hierarchical directory structure where each folder has a specific purpose for system operation, user data, and application management.

Basic linux commands 

## to switch the user 
```bash
sudo -i
```
## to check the present working directory 
```bash
pwd
```
## to check the os information
```bash
cat /etc/os-release
```
## to list the files or directories
```bash
ls
```
## Show hostname 
```bash
hostname
```
## used to clear the terminal 
```bash
clear
```
## to show the command description or open the manual for specific command 
```bash
man<command>
```
## to display free memory 
```bash
free-h
```
## to change the directory 
```bash
cd
```
## to check current shell 
```bash
echo $shell
```
## to check the cpu information 
```bash
lscpu
```
## to check the block devices 
```bash
lsblk
```
## to check the size of the file or directory
```bash
du-sh /filename or /dirname
```
## to check disk file info  
```bash
df -h
```

