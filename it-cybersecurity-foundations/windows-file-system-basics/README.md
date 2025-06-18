## Windows File System Basics

In this lab I focused on understanding how Microsoft Windows structures and manages files, directories, system configurations, and hidden behaviors across its file system. I explored key areas such as system folders, user profiles, logs, startup behavior, registry structure, environmental variables, and unique NTFS features like Alternate Data Streams.

### What I Learned
- Structure and function of Windows system directories like `System32`, `Users`, `Program Files`, `AppData`, and `Windows`
- Role and location of hidden system files and critical logs
- How the registry is structured and accessed via `regedit`
- Use and security implications of the SAM database
- Environment variables, especially the `PATH` variable
- How startup apps are registered and triggered
- Windows NTFS Alternate Data Streams 
- How Windows maps file types to default applications

### Key Activities

| Task | Tools / Path | Outcome |
|------|--------------|---------|
| Examined Startup folder | `shell:startup` | Learned how apps auto launch for a user |
| Created a batch file | `test.bat` | Saw it show up as a startup app |
| Explored the SAM database | `C:\Windows\System32\config\SAM` | Understood its secure nature and role in storing credentials |
| Viewed Registry hives | `regedit` | Located `SECURITY`, `SYSTEM`, and `SOFTWARE` hives |
| Viewed system logs | `Event Viewer` | Located `.evtx` log files and understood their format |
| Inspected `System32` | `C:\Windows\System32` | Saw `.dll` and `.exe` files for essential tools |
| Explored the PATH variable | `echo %PATH%`, `sysdm.cpl` | Compared system vs user level path entries |
| Created an ADS file | `notasecret.txt:secret` | Used PowerShell to view hidden stream |
| Read hosts file | `C:\Windows\System32\drivers\etc\hosts` | Understood how it can override DNS |
| Mapped file extensions | `Default Apps` settings | Learned how file types are linked to apps |

### Tools Used
- Windows File Explorer
- CMD & PowerShell
- Event Viewer
- Registry Editor
- System Properties & Environment Variables UI

---

