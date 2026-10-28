Lab 7: Network Connectivity Troubleshooting
Ticket Information
Ticket ID: LAB-007
Category: Network Connectivity / DNS
Environment: Simulated Windows 11 workstation
Priority: Medium (simulated)
Status: Resolved (simulated)
Technician: IT Support Trainee
1. Issue Description
The user reported that the computer was connected to Wi-Fi but could not access any websites.

The issue began that morning. Another laptop connected to the same Wi-Fi network was able to browse normally.

2. Initial Assessment
Initial questions established that:

The affected computer showed a Wi-Fi connection.
No websites loaded in the browser.
Another device on the same Wi-Fi network could access websites.
These findings suggested that the issue was likely specific to the affected workstation.

3. Troubleshooting Steps
Step 1: Inspect IP Configuration
Command:

ipconfig
Findings:

IPv4 address: 169.254.18.42
Subnet mask: 255.255.0.0
Default gateway: Missing
Assessment: The APIPA address and missing default gateway suggested that the workstation had failed to obtain a valid IPv4 configuration from DHCP.

Step 2: Renew the IP Address
Commands:

ipconfig /release
ipconfig /renew
Result: The workstation obtained the following configuration:

IPv4 address: 192.168.1.25
Subnet mask: 255.255.255.0
Default gateway: 192.168.1.1
This restored a valid-looking network configuration.

Step 3: Test Network Connectivity
Commands:

ping 192.168.1.1
ping 8.8.8.8
nslookup google.com
Results:

Default gateway: Successful
External IP address: Successful
DNS lookup: Failed
Assessment: The workstation could communicate with its gateway and reach an external IP address, but DNS resolution was failing.

Step 4: Investigate DNS
Command:

ipconfig /all
The configured DNS server was 192.168.1.250.

Targeted DNS test:

nslookup google.com 192.168.1.250
Result: DNS requests timed out.

An alternate lookup against 8.8.8.8 succeeded in the simulation.

Assessment: The results indicated a likely problem with the configured DNS server or its network path. The exact underlying cause was not independently established.

Step 5: Apply the Approved Correction
The simulated IT administrator authorized correcting the DNS configuration to the approved DNS settings.

The correction was applied according to the simulated organization’s network policy.

Step 6: Verify Resolution
The following checks were completed:

Gateway connectivity test: Successful
External IP connectivity test: Successful
DNS lookup: Successful
Browser test: Websites loaded normally
User confirmation: The user confirmed that browsing worked again
4. Root Cause Assessment
The incident involved two observed network issues:

An initial APIPA address and missing default gateway, consistent with a failure to obtain a DHCP-assigned IPv4 configuration.
Subsequent DNS lookup failures involving the configured DNS server.
The evidence supports a DNS configuration or DNS server connectivity issue after the IP configuration was renewed. The precise cause of the initial DHCP failure and the DNS failure was not conclusively determined.

5. Resolution
Released and renewed the workstation’s IP configuration.
Verified local gateway and external IP connectivity.
Investigated the configured DNS server using a targeted lookup.
Applied the administrator-approved DNS correction in the simulation.
Retested connectivity and confirmed successful DNS resolution and web browsing.
6. Final Outcome
Status: Resolved in the simulated environment.

The workstation successfully resolved domain names and accessed websites after the approved correction. The user confirmed that service was restored.

7. Skills Practiced
Windows command-line troubleshooting
IPv4 addressing and APIPA
DHCP troubleshooting
Default gateway identification
Basic connectivity testing with ping
DNS diagnosis using nslookup
Network configuration verification using ipconfig /all
Following change authorization and documenting results
User confirmation and ticket closure
8. Lessons Learned
A Wi-Fi connection indicator does not guarantee internet access. Troubleshooting should proceed systematically from IP configuration to gateway connectivity, external IP connectivity, and DNS resolution.

Changes to managed DNS settings should follow organizational policy. A ticket should document the evidence, corrective action, verification results, and user confirmation before closure.



