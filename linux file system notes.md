📁 Lab Notes: Linux File System Basics
💡 Lab Overview
Completed a guided hands-on Linux lab focused on exploring the Linux file system using command-line tools. Practiced navigation, understood key directories, and examined devices, logs, and processes.

🔍 Exploring the Linux File System
Navigated to the root directory with: cd /

Listed contents using: ls -l

d = directory (e.g., /home, /etc)

l = symbolic link

rwx = permissions (read, write, execute)

🌲 Tree Structure Navigation
Viewed root tree structure: tree / -L 1

Explored home directories: tree /home

Created new user with home directory: sudo adduser michael

📁 Key Directories and Their Purpose
Directory	Description
/etc	System configuration files (hosts, fstab, crontab)
/var/log	System logs (syslog, auth.log, dmesg, etc.)
/usr	Shared user tools, binaries, libraries, docs
/opt	Third-party applications (e.g., Oracle)
/dev	Device files (e.g., /dev/null, /dev/xvda)
/mnt	Mount point for external drives (USB, CD, NFS)
/root	Home directory for the root user
/proc	Virtual file system with running processes
/boot	Boot files (e.g., kernels, initrd)

🔧 Storage & Devices
Listed disk partitions: sudo fdisk -l | grep dev | grep -v loop

Checked mounted partitions: sudo df -h

Listed block devices: lsblk

📝 Logs & Monitoring
Viewed kernel messages: sudo last, sudo who

Monitored system logs live: sudo tail -f /var/log/syslog

