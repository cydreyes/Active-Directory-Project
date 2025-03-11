# Active Driectory Project

## Objective

This project establishes a virtualized environment using Oracle VM VirtualBox, incorporating Windows 10, Kali Linux, Windows Server, and Ubuntu Server virtual machines. Network configurations facilitate communication through IP addressing and NAT Networks. Security measures include a Splunk Server for log analysis, a Universal Forwarder for data transmission, and Sysmon for endpoint monitoring. Testing methodologies involve Hydra for brute-force attack simulations, Atomic Red Team (ART) for security assessments, and Splunk for log analysis. Windows machines are integrated into an Active Directory domain with Remote Desktop enabled. PowerShell scripting automates various tasks, providing a hands-on approach to exploring cybersecurity tools and concepts within a controlled environment.


### Skills Learned
[Bullet Points - Remove this afterwards]

- Virtualization: Configured and managed virtual machines (Windows 10, Kali Linux, Windows Server, Ubuntu Server) using Oracle VM VirtualBox.
- Network Configuration: Assigned IP addresses, implemented NAT Networks, and troubleshot connectivity issues (ping tests, DNS resolution).
- Log Management & Analysis: Deployed and configured Splunk Server and Universal Forwarder for centralized log collection and analysis.
- Endpoint Security: Implemented Sysmon for advanced event logging and endpoint monitoring.
- Security Testing & Adversary Simulation: Conducted brute-force attack simulations using Hydra and executed adversary emulation scenarios with Atomic Red Team (ART).
- Threat Detection & Incident Response: Analyzed security event logs in Splunk, focusing on authentication events (e.g., Event IDs 4625 - failed logins, 4624 - successful logins).
- Active Directory Administration: Joined Windows machines to a domain and configured domain-based authentication.

### Tools Used
[Bullet Points - Remove this afterwards]

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
## Steps


![Diagram](https://github.com/user-attachments/assets/39e22a7a-1fbc-417c-9b4d-d78c57aa1eea)

### Part 1: Installing the VMs

### Hardware Requirements
- To run this lab smoothly, it is recommended to have:
- At least 16GB of RAM.
- 250GB of disk space.
- A Windows machine (using VirtualBox for virtualization).

### Step 1: Install VirtualBox
1. Download and install Oracle VirtualBox from the official website.

### Step 2: Install Windows 10
1. Go to  https://www.microsoft.com/en-ca/software-download/windows10, to get ISO file
2. Create a new VM, use the following:
- Name: Windows 10
- Memory: 4GB
- CPU: 1
- Storage: 50GB
3. Attach the ISO file
4. After installation, create a local user account

### Step 2: Install Kali Linux
1. Go to  https://www.kali.org/
2. Extract using 7-zip, start the VM
3. Log in with
- username: kali
- password: kali
4. After installation, update the system:
   ```bash
   sudo apt update && sudo apt upgrade -y
### Step 3: Install Windows Server
1. Download the ISO file from https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022
2. Create a new VM, use the following:
- Memory: 4GB
- CPU: 1
- Storage: 50GB
3. Start the VM, choose "Windows Server 2022 Standard Evaluation (Desktop Experience)
4. Create a user and passowrd 

### Step 4: Install Ubuntu Server 
1. Go to https://ubuntu.com/server
2. Download the latest version
3. Create a new VM, use the following:
- Memory: 8GB
- CPU: 2
- Storage: 100GB
4. Start the VM and follow installation steps
5. Set up a user and password
6. After installation, update the system:
   ```bash
   sudo apt update && sudo apt upgrade -y

### Part 2: Install & Configure Sysmon & Splunk 
