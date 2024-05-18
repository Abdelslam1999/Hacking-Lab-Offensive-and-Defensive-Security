# Hacking-Lab-Offensive-and-Defensive-Security
This project demonstrates a home lab setup with two virtual machines: one running Windows 10 (defender) and another running Kali Linux (attacker). The goal is to showcase various attack and defense techniques in a controlled environment.

**CAUTIONS** ⚠️⚠️
"THIS PROJECT REQUIRES A CAPABLE DEVICE FOR THE VIRTUAL MACHINES TO WORK SIMULTANEOUSLY TRYING TO DO IT WITH A WEAK DEVICE MIGHT RESULT IN OVERHEATING"

**Setup and Configuration**
- **Tools and Software**:
- Virtualization Software (e.g., VirtualBox, VMware)
- Windows 10 ISO
- Kali Linux ISO
- Networking setup (e.g., Host-only Adapter)


**Virtual Machine Configuration**
**Windows 10 VirtualBox**
- *Installation Steps*:
  1. Download the Windows 10 ISO.
  2. Create a new virtual machine in VirtualBox.
  3. Follow the installation wizard to set up Windows 10.
- *Configuration*:
  - Configure network settings to use Host-only Network Adapter.
  - Create a user account with administrative privileges.
  - Enable Windows Defender and Firewall.

**Kali Linux VirtualBox**
- *Installation Steps*:
  1. Download the Kali Linux ISO.
  2. Create a new virtual machine in VirtualBox.
  3. Follow the installation wizard to set up Kali Linux.
- *Configuration*:
  - Configure network settings to use Host-only Network Adapter.
  - Update the system and install essential tools (`sudo apt update && sudo apt install nmap metasploit-framework`).
  - ![4](https://github.com/Abdelslam1999/Hacking-Lab-Offensive-and-Defensive-Security/assets/97275603/12e4f11d-79b4-4087-b938-873407965d00)

**why did I choose host only network???**<br>
  -The first reason is for the host and virtual machines to be able to see each others in the network.
  -secondly for the virtual machine to be connected to the internet that will be a big red flag for       our machine is vulnerable because we going to exposed to alot of vulnerabilities and malicious         software. 
  -isolate the virtual machines with their own network for the devices to see each other.
![5](https://github.com/Abdelslam1999/Hacking-Lab-Offensive-and-Defensive-Security/assets/97275603/dbaa84bc-a612-4dff-beff-f36cbb46a6ee)
**Windows 10 virtual machine (defensive)**
![6](https://github.com/Abdelslam1999/Hacking-Lab-Offensive-and-Defensive-Security/assets/97275603/b5f16807-0e4e-467a-926a-8798492b122a)
**Kali Linux Virtual machine (offensive)**

**skills and project to do in Sandbox**

  **Attack Scenarios**<br>
  **Scenario 1: Reconnaissance**
- **Objective**: Gather information about the target (Windows 10 VM)
- **Tools**: Nmap, Netcat
 
 - **Steps**:
1. Perform network scanning with Nmap
2. Document open ports and services<br>

**Scenario 2: Vulnerability Scanning**
- **Objective**: Identify vulnerabilities in the target system
- **Tools**: OpenVAS, Nessus
 
 - **Steps**:
1. Configure and run a vulnerability scan
2. Analyze the scan results<br>

**Scenario 3: Exploitation**
- **Objective**: Exploit a discovered vulnerability
- **Tools**: Metasploit Framework
 
 - **Steps**:
1. Select and configure an exploit
2. Execute the exploit and gain access
3. Demonstrate a simple payload (e.g., reverse shell)

 **Defense Strategies**<br>
**Scenario 1: Hardening the System**
- **Objective**: Implement security measures to protect the Windows 10 VM
 
 - **Steps**:
1. Enable and configure Windows Firewall
2. Install and configure antivirus software
3. Apply system and software updates

**Scenario 2: Intrusion Detection**
- **Objective**: Detect malicious activities on the network
- **Tools**: Wireshark, Snort
 
 - **Steps**:
1. Set up and configure Snort for intrusion detection
2. Monitor network traffic and identify suspicious activities



