#  Key Concepts and Commands Practiced: Linux CLI Basics Lab

 **Basic Navigation & Identification**
- Identified user and system info using: `whoami`, `hostname`, `pwd`, `id`
- Navigated the file system using: `cd`, `cd ..`, `pwd`, `ls`

 **Understanding Files and Permissions**
- Used `ls -l` to view file permissions like `drwxr-xr-x`
- Understood file permission groups: owner, group, others
- Recognized the difference between files and directories using symbols (`-`, `d`)

 **Creating and Modifying Files**
- Created folders using `mkdir`
- Created empty files using `touch`
- Appended content using `echo "text" >> file.txt`
- Displayed file contents using `cat`

 **File Management**
- Copied files using `cp`
- Moved and renamed files using `mv`
- Removed files safely with `rm -i`

 **Working with Large Files**
- Viewed long content using `more` and `less`
- Used `base64 /dev/urandom | head -c 1M > abigfile.txt` to generate a large random file

 **Searching and Parsing**
- Searched for files by name with `find`
- Found text inside files using `grep`
- Combined commands using `|` (pipes) for parsing:
  - `sort`, `uniq`, and `wc` for filtering and counting
