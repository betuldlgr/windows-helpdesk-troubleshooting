# windows-helpdesk-troubleshooting
Step-by-step troubleshooting of common Windows IT Help Desk issues, documented through real-world scenarios.
## Scenario 1: Wi-Fi Connected but No Internet

**Issue:**  
User reports that the computer is connected to Wi-Fi, but there is no internet access.

**Initial Checks:**  
- Confirmed Wi-Fi connection status  
- Asked user if issue affects other devices  

**Troubleshooting Steps:**  
1. Ran `ipconfig` to verify IP address  
2. Checked if the device received an APIPA address (169.254.x.x)  
3. Verified DNS server configuration  
4. Restarted the network adapter  

**Root Cause:**  
Incorrect DNS configuration causing failure to resolve domain names.

**Resolution:**  
Updated DNS settings to obtain DNS automatically and reconnected to the network.

**What I Learned:**  
This issue highlighted the importance of DNS in network connectivity and reinforced a structured troubleshooting approach.

## Scenario 2: Computer Running Very Slowly

**Issue:**  
User reports that the computer is extremely slow during normal use.

**Initial Checks:**  
- Asked when the issue started  
- Confirmed whether the issue occurs after startup or during specific tasks  

**Troubleshooting Steps:**  
1. Opened Task Manager to identify high CPU, memory, or disk usage  
2. Reviewed startup applications and disabled unnecessary programs  
3. Checked available disk space  
4. Restarted the system after changes  

**Root Cause:**  
Too many startup applications consuming system resources.

**Resolution:**  
Disabled non-essential startup programs, resulting in improved system performance.

**What I Learned:**  
This scenario reinforced the importance of checking system resources and startup processes when troubleshooting performance issues.

## Scenario 3: Printer Not Printing / Not Showing

**Issue:**  
User reports that the printer is not printing or does not appear in the list of available printers.

**Initial Checks:**  
- Confirmed whether the printer is powered on  
- Verified physical connections or network connectivity  
- Asked if other users are experiencing the same issue  

**Troubleshooting Steps:**  
1. Checked printer status in Devices and Printers  
2. Restarted the Print Spooler service  
3. Verified that the correct printer driver was installed  
4. Removed and re-added the printer  

**Root Cause:**  
Print Spooler service was not running, preventing print jobs from being processed.

**Resolution:**  
Restarted the Print Spooler service and successfully restored printing functionality.

**What I Learned:**  
This scenario demonstrated the importance of checking Windows services when troubleshooting printer-related issues.


