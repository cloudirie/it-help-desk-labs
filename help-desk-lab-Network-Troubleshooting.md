# Help Desk Lab 12 — Network Connectivity Troubleshooting

## Ticket Title
Employee Unable to Access Company Shared Drive

## 1. Issue Reported
Employee reported being unable to access company shared files despite having an active Wi-Fi connection.

## 2. Troubleshooting Performed
- Ran `ipconfig` to inspect the computer's IP configuration.
- Used `ping` to test connectivity to the default gateway.
- Used `ping 8.8.8.8` to test external connectivity.
- Used `nslookup` to test DNS resolution.
- Compared network configurations with a working employee's computer.
- Identified that the affected computer was connected to Guest Wi-Fi instead of Corporate Wi-Fi.

## 3. Root Cause
The employee's computer was connected to the Guest Wi-Fi network, which did not provide access to internal company resources.

## 4. Resolution
Guided the employee to disconnect from Guest Wi-Fi and connect to the authorized Corporate Wi-Fi network.

Verified internal DNS resolution and confirmed that access to the shared drive was restored.

## 5. Ticket Status
**Resolved** — Employee confirmed successful access to company shared files.

## Commands Practiced
```cmd
ipconfig
ping 192.168.1.1
ping 8.8.8.8
nslookup google.com
nslookup fileserver.company.local
```

## Skills Practiced
- IP configuration troubleshooting
- Default gateway connectivity testing
- Network connectivity testing
- DNS troubleshooting
- Network configuration comparison
- Wi-Fi troubleshooting
- Incident documentation
