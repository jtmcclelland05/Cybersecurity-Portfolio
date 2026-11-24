**Lab 01 - Failed Logon Detection**

**Objective**

The goal of this lab was to generate failed authentication attempts in a Windows Active Directory environment and investigate the resulting security events.

**Tools Used**

- Windows Server 2022
- Windows 11 Pro
- Active Directory
- Windows Event Viewer
- Wazuh SIEM
- Oracle VirtualBox

**Lab Procedure**

1. Verified connectivity between the Windows endpoint and domain controller.
2. Verified that the Wazuh agent was active.
3. Generated failed login attempts using incorrect credentials.
4. Opened Windows Event Viewer to investigate authentication failures.
5. Identified relevant Windows security event IDs.
6. Reviewed security monitoring activity in the Wazuh dashboard.

**Security Events Identified**

| Event ID | Description |
| --- | --- |
| 4625 | Failed account logon |
| 4771 | Kerberos pre-authentication failure |

**Investigation**

During the investigation, I reviewed authentication failure events and examined their source IP addresses.

One of the addresses identified was 192.168.56.101, which belongs to my Windows 11 endpoint.

I also encountered the address ::ffff:192.168.56.101 and learned that this represents an IPv4-mapped IPv6 address.

**Findings**

- Failed authentication attempts generated Windows security events.
- Event ID 4625 indicated an unsuccessful login attempt.
- Event ID 4771 indicated a Kerberos pre-authentication failure.
- Source IP addresses helped identify where authentication attempts originated.

**What I Learned**

This lab helped me understand how Windows records authentication failures and how security analysts can investigate suspicious login activity. Repeated authentication failures can be an indicator of a brute-force attack, although additional investigation is needed to determine whether the activity is malicious.

**Screenshots**

Screenshots will be added after repeating the authentication tests.
