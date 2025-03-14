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
