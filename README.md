# What is IR-Flash ?
Automated Script to capture forensic evidences (logs) from an Windows EndPoint. You do not need any hitups while collecting the logs. Just need to run the IR-dump.bat script with the administrative privilege. And see the script doing all the magic.
* In return get me some subscribers for my YouTube Channel 👉 https://www.youtube.com/c/BlackPerl
* If you like to support my creation and pay me back a little, you can buy me a coffee ☕ https://www.buymeacoffee.com/BlackPerl

# What we are capturing here ?
  1. arp table of the current network
  2. ipconfig of this machine
  3. dnscache
  4. ipv4 stack from netsh
  5. firewall settings from netsh
  6. wifi configuration from netsh (no passwords)
  7. System Information
  8. Service list
  9. Process list
  10. Eventlogs- (Application, Security, PS), Defenderlogs, Firewalllogs
  11. GPO (text and HTML)
  12. Windows Scheduler
  13. Audit Policy
  14. net user
  15. net localgroups
  16. net session
  17. net share
  18. doskey /history
  19. powershell logs for all users where accessible
  20. Registry
  21. AV Vendor logs (Cylance, McAfee, Defender, TrendMicro)- If exists
  22. Firewall eventlog
  23. registry backup
  24. WMI consumer
  25. archive of local scripts

# How to use this ?
  1. Open a CMD prompt with Administrive privilege on the machine from which you need to gather the logs
  2. Extract the IR-Dump.zip file
  3. CD to the location where you have saved the file
  4. Run- "IR-dump.bat" (Detailed logs too big for email but great for malware diags)
  5. Run- "IR-dump.bat /m" (As above but also captures a memory dump)
  6. Run- "IR-dump.bat /s" (Small eventvwr logs only - if you're short of space fits into email but not much details)
  7. Run- "IR-dump.bat /f" (Also captures file system permissions (slow))
  8. Run- "IR-dump.bat /h" (Capures with windows file system hashes (very slow))
  9. Run- "IR-dump.bat /f /m /h" (All options above (Very Very Slow you probably don't want this), but can be done while needed)
