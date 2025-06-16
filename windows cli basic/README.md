# Windows CLI Basics Lab

In this lab I worked on fundamental command line skills in Windows using both the traditional CLI and PowerShell. It was divided into three key sections: navigation, file operations, and system administration.

---

## Navigation Commands

| Command | Purpose |
|--------|---------|
| `whoami` | Shows current user. |
| `cd %HOMEPATH%` | Navigates to user’s home directory. |
| `dir` | Lists contents of the current directory. |
| `tree` | Shows directory structure in tree format. |
| `help dir` | Displays help info for the `dir` command. |
| `dir /s /p` | Recursively lists all files/folders with pause between pages. |

---

## File Operations

| Command | Purpose |
|---------|---------|
| `mkdir apple1 apple2 apple3` | Creates three folders. |
| `echo The cow says moo. > apple1\cow.txt` | Writes a string to `cow.txt`. |
| `type apple1\cow.txt` | Displays contents of the file. |
| `>>` | Appends text to a file. |
| `copy apple1\cow.txt apple2\notacow.txt` | Copies file with a new name. |
| `dir /s /b \| findstr apple \| findstr .txt` | Finds all `.txt` files in apple directories. |
| `rename apple2\notacow.txt reallyacow.txt` | Renames a file. |
| `move apple3\manycows.txt apple2` | Moves file to another directory. |
| `del apple2\manycows.txt` | Deletes the file permanently. |
| `mkdir one\two\three` | Creates nested directories. |
| `rmdir /s one` | Deletes a directory and its subfolders. |
| `doskey /history` | Shows current CLI session history. |

---

## System Administration

| Command | Purpose |
|---------|---------|
| `systeminfo` | Displays OS version, system configuration, memory, etc. |
| `tasklist` / `tasklist /v` | Lists running processes. |
| `date /t` & `time /t` | Displays system date and time. |
| `sc query` / `sc query wscsvc` | Shows Windows service status. |
| `net`, `net share`, `net user`, `net localgroup` | Manages shares, users, groups. |
| `net accounts` | Shows password policies. |
| `net user \| find /c /v ""` | Attempts to count user accounts. |
| `net localgroup \| find /c "*"` | Counts local groups. |
| `net share \| find /c "$"` | Counts hidden admin shares. |
| `ipconfig` | Shows IP address and network info. |
| `for /L %a in (1,1,255) do @ping -n 1 -w 10 x.y.z.%a > nul && echo x.y.z.%a is up!` | Performs a ping sweep on local subnet. |
| `ping 8.8.8.8` | Tests connectivity to Google DNS. |
| `nslookup www.moo.com 8.8.8.8` | Resolves domain to IP using DNS. |
| `netstat -ant` | Displays open network connections and listening ports. |

---

## Skills Practiced

- Windows navigation using CLI
- File creation, manipulation, and deletion
- Pattern searching using `findstr` and `find`
- Understanding hidden shares, groups, users
- Basic Windows service inspection
- Networking tools for enumeration and troubleshooting

---

