# Project Findings
___
## Splunk Server
Splunk was installed on the Ubuntu server. In the Ubuntu server, a static ip was set by modifying this file:
```bash
sudo nano /etc/netplan/50-cloud-init.yaml
```
Inserting:
![netplan](https://github.com/user-attachments/assets/b91b19f8-a914-4ce1-ab76-70e9833fd909)

The Splunk interface can be accessed via a web browser at **192.16810.10:8000**. An index **"endpoint"** was created to receive logs from the 
Active Directory server and the Windows target machine. 
![Splunk123](https://github.com/user-attachments/assets/a7e6383b-e0a7-41a4-b89e-ad9149c458f3)

## Active Directory
In the Windows Server VM, I used Active Directory services and created a domain called **"cerberus.local"** and I added the Windows 10 workstation to it. 
![AD1](https://github.com/user-attachments/assets/5bfb5ecf-c3f6-4030-a364-1d4f6c016401)

I created Organizational units called **"HR"** and **"IT"**. For HR, I created two users **Lebron James** and **Terry Smith**. For IT, I created three users **Jenny Smith, Kobe Bryant,** and **Michael Jordan**. 
![AD2](https://github.com/user-attachments/assets/0448febc-dfc4-49ee-ae2c-cec02ff3b195)

I gave all users permission to **RDP** to the Windows 10 workstation. 

![rdp](https://github.com/user-attachments/assets/c4d554fe-3a6b-40f8-9ce1-e7bd0f18c280)

## Simulated Attack
Since I gave all users permission to RDP, I used **Kali Linux** to simulate a dictionary password attack on **Michael Jordan**. I used a predefined list of passwords
on Kali Linux and saved it to a file called **"passwords.txt"**. I inserted Michael Jordan's password into that file and used **hydra** to perfom the attack. 
![hydra](https://github.com/user-attachments/assets/1cd88aff-91d8-4b7e-bf29-e3ce4e26c723)

### Splunk Log 
I then went on Splunk and searched for logs that included ***mjordan*** and the **EventCode=4624** which indicates a successful remote desktop logon. 
![splunk-4624](https://github.com/user-attachments/assets/0f2e5ff5-b651-47fc-ba7f-6dad0cc95576)
