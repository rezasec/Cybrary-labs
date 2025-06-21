# Log Analysis Basics

In this lab, I worked through a set of VPN authentication logs using basic Linux commands to figure out what was happening. The goal was to identify successful logins by “test” users, track the IP addresses they came from, and see if any other accounts were using those same IPs.

---

### Log Analysis Workflow:
1. Defined the analysis objective.
2. Identified the relevant log file.
3. Verified time coverage.
4. Measured file size and line count.
5. Previewed file structure and contents.
6. Used targeted searches to extract useful data.

### Tools & Commands Practiced:
- Navigated directories and examined files with `cd`, `ls -lah`, `file`
- Read and scoped log contents using `cat`, `head`, `tail`
- Counted lines with `wc -l`
- Searched log data using `egrep -i` for pattern matching
