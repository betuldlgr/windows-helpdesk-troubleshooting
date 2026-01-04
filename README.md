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
