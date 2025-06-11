📚 Lab Notes: Linux File System Basics
Completed a hands on lab focused on understanding the Linux file system structure, storage management, and log monitoring. This session helped clarify how Linux organizes files, devices, and critical system paths.

✅ Key Concepts and Commands Practiced
🔍 Exploring the File System
Navigated to the root directory using cd /

Used ls -l to display directory contents and symbolic links

Learned:

d = directory (e.g., /home, /etc)

l = symbolic link (shortcut)

rwx = read, write, execute permissions

🌲 Tree Structure Navigation
tree / -L 1: Viewed the root directory one level deep

tree /home: Listed all home user folders

sudo adduser michael: Created a new user and verified the home directory was auto-created

📁 Key Linux Directories and Their Roles
/etc: Stores system config files (e.g., hosts, fstab, crontab)

/var/log: System logs like syslog, auth.log, dmesg

/usr: Shared user tools, binaries, docs, libraries

/opt: Reserved for third-party applications

/dev: Device files (e.g., /dev/null, /dev/xvda)

/mnt: Mount point for external devices (USB, CD, NFS)

/root: Home directory for the root user

/proc: Temporary virtual filesystem showing running processes

/boot: Stores boot files used during startup

💽 Disk & Storage Management
sudo fdisk -l | grep dev | grep -v loop: Listed physical storage devices

sudo df -h: Checked disk usage in human-readable format

lsblk: Listed block devices and mount points

🛠️ Log Monitoring & System Tools
sudo tail -f /var/log/syslog: Monitored live system logs

sudo last: Viewed login history

sudo who: Checked currently logged-in users

