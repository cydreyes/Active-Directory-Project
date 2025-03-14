# Active Directory Project
Special thanks to **MyDFIR** for the tutorial for this project. https://www.youtube.com/@MyDFIR

## Objective

This project establishes a virtualized environment using Oracle VM VirtualBox, incorporating Windows 10, Kali Linux, Windows Server, and Ubuntu Server virtual machines. Network configurations facilitate communication through IP addressing and NAT Networks. Security measures include a Splunk Server for log analysis, a Universal Forwarder for data transmission, and Sysmon for endpoint monitoring. Testing methodologies involve Hydra for brute-force attack simulations, Atomic Red Team (ART) for security assessments, and Splunk for log analysis. Windows machines are integrated into an Active Directory domain with Remote Desktop enabled. PowerShell scripting automates various tasks, providing a hands-on approach to exploring cybersecurity tools and concepts within a controlled environment.


### Skills Learned

- Virtualization: Configured and managed virtual machines (Windows 10, Kali Linux, Windows Server, Ubuntu Server) using Oracle VM VirtualBox.
- Network Configuration: Assigned IP addresses, implemented NAT Networks, and troubleshot connectivity issues (ping tests, DNS resolution).
- Log Management & Analysis: Deployed and configured Splunk Server and Universal Forwarder for centralized log collection and analysis.
- Endpoint Security: Implemented Sysmon for advanced event logging and endpoint monitoring.
- Security Testing & Adversary Simulation: Conducted brute-force attack simulations using Hydra and executed adversary emulation scenarios with Atomic Red Team (ART).
- Threat Detection & Incident Response: Analyzed security event logs in Splunk, focusing on authentication events (e.g., Event IDs 4625 - failed logins, 4624 - successful logins).
- Active Directory Administration: Joined Windows machines to a domain and configured domain-based authentication.

### Tools Used


- Oracle VM VirtualBox Manager – Creates and manages virtual machines (VMs).
- Splunk Server – Analyzes and monitors security logs.
- Splunk Universal Forwarder – Forwards log data to Splunk for centralized analysis.
- Sysmon – Provides endpoint monitoring and detailed logging on Windows machines.
- Hydra – Simulates brute-force attacks for security testing.
- Atomic Red Team (ART) – Conducts security testing and validation.
- PowerShell – Automates administrative and security tasks.
- Microsoft Windows Event Logs – Analyzed within Splunk for security monitoring and threat detection.
- Windows Server 2022 – Configured for Active Directory Domain Services (AD DS).
- Ubuntu Server – Functions as the Splunk server within the lab environment.
- Microsoft Windows 10 – Used as the primary target machine for security testing.
- Kali Linux – Serves as the attacker machine for penetration testing and simulations.
## Network Topology


![Screenshot 2025-03-11 204536](https://github.com/user-attachments/assets/41a435aa-9064-4ea6-a250-9ae66be5447f)


