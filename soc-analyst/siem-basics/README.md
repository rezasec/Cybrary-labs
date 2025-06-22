# SIEM Basics

I explored how a SIEM platform works by using Wazuh to search, filter, and investigate log data. I started by exploring existing security alerts in the Wazuh dashboard and ran a simulated brute force attack to see how a SIEM helps detect suspicious activity.

---

## Summary

### Exploring the SIEM  
- Used Wazuh’s dashboard to examine over 700 existing security events from a set date range.  
- Learned to filter out low priority alerts using filter tools.  
- Focused on potentially serious alerts

### Simulating an Attack  
- Ran a simulated brute force SSH attack using a script in the terminal.  
- Reviewed fresh log alerts in real time 
- Tracked attack patterns by identifying:
  - The rule ID (`5716`) tied to failed SSH logins  
  - The location field showing where the logs came from  
  - Timestamps of the first and last login failures  

---

## Skills Practiced

| Skill                  | Description                                                                  |
|------------------------|------------------------------------------------------------------------------|
| SIEM Navigation        | Explored Wazuh’s Security Events dashboard and used Lucene syntax            |
| Log Filtering          | Removed noisy logs and low level events to focus on critical alerts          |
| Alert Analysis         | Analyzed alert details such as `rule.id`, `location`, and MITRE techniques   |
| Brute Force Detection  | Detected and investigated SSH brute force attempts through log correlation   |
