# 📚 Lab Notes: Linux File System Basics

Completed a hands on guided lab focused on understanding the Linux file system structure, storage management, and log monitoring. This session helped clarify how Linux organizes files, devices, and critical system paths.

---


### ✅ Key Concepts and Commands Practiced

---

### 🔍 Exploring the File System
- Navigated to the root directory using `cd /`
- Used `ls -l` to display directory contents and symbolic links
- Learned:
  - `d` = directory (e.g., `/home`, `/etc`)
  - `l` = symbolic link (shortcut)
  - `rwx` = read, write, execute permissions

---

### 🌲 Tree Structure Navigation
- `tree / -L 1`: Viewed the root directory one level deep
- `tree /home`: Listed all home user folders
- `sudo adduser michael`: Created a new user and verified the home directory was auto-created

---

### 📁 Key Linux Directories and Their Roles
- `/etc`: System config files like `hosts`, `fstab`, `crontab`
- `/var/log`: System logs (e.g., `syslog`, `auth.log`, `dmesg`)
- `/usr`: Shared user tools, binaries, docs, libraries
- `/opt`: Third-party software installations
- `/dev`: Device files (`/dev/null`, `/dev/xvda`, etc.)
- `/mnt`: Mount point for USB, CDs, external drives
- `/root`: Home directory for the root user
- `/proc`: Virtual filesystem showing running processes
- `/boot`: Boot files needed during startup

---

### 💽 Disk & Storage Management
- `sudo fdisk -l | grep dev | grep -v loop`: List physical drives
- `sudo df -h`: View partitions and usage in human-readable format
- `lsblk`: List block devices and mount points

---

### 🛠️ Log Monitoring & System Utilities
- `sudo tail -f /var/log/syslog`: Monitor real-time system logs
- `sudo last`: View login history
- `sudo who`: Show current logged-in users

---

💬 _This lab gave me a much clearer understanding of how Linux organizes data and devices, and how to monitor and explore system behavior through logs and commands._  
