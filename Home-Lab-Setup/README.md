**SOC Home Lab Setup**

**Overview**

I built this home lab using Oracle VirtualBox to practice security monitoring, log analysis, endpoint security, and network intrusion detection in an isolated environment.

**Virtual Machines**

| Machine | Operating System | IP Address | Purpose |
| --- | --- | --- | --- |
| DC01 | Windows Server 2022 | 192.168.56.20 | Active Directory and DNS |
| WIN11-ENDPOINT | Windows 11 Pro | 192.168.56.101 | Endpoint monitoring and security testing |
| Wazuh Server | Ubuntu Server | 192.168.56.10 | SIEM and security monitoring |

**Network Configuration**

- Virtualization platform: Oracle VirtualBox
- Network type: Host-only
- Subnet: 192.168.56.0/24
- Subnet mask: 255.255.255.0
- Active Directory domain: corp.lab.test

**Security Tools**

- Wazuh - Security monitoring and log analysis
- Microsoft Defender - Endpoint protection
- Wireshark - Network packet analysis
- Suricata - Network intrusion detection
- Windows Event Viewer - Windows security event analysis

**Lab Capabilities**

- Monitor failed authentication attempts
- Investigate Windows security events
- Detect and analyze endpoint malware alerts
- Capture and inspect network traffic
- Generate network intrusion detection alerts

**Network Architecture**

A network diagram and screenshots of the lab environment will be added as I continue documenting the setup.
