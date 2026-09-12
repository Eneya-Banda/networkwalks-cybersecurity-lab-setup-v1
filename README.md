# networkwalks-cybersecurity-lab-setup-v1
This repository documents my learning journey and practical work as I undertake a Cybersecurity Internship Program with Network Walks.  The purpose of this repository is to build and demonstrate hands-on skills in cybersecurity, ethical hacking, network security, vulnerability assessment, system security, and security best practices.
# Project Overview
This project documents the setup and development of a virtual Cybersecurity and Ethical Hacking Testing Lab using Oracle VirtualBox and Kali Linux.

The purpose of this lab is to create a controlled and isolated environment for learning and practising cybersecurity concepts, network security, vulnerability assessment, penetration testing and ethical hacking techniques.
# Objectives
- Set up a cybersecurity testing environment using VirtualBox.
- Install and configure Kali Linux as the primary security-testing machine.
- Configure a custom NAT using the 10.0.0.0/24 subnet.
- Configure Kali Linux with the IP address 10.0.0.2/24.
- Enable internet connectivity for the Kali Linux VM.
- Create VM Snapshots to provide recovery points.
- Document the complete setup process.
- Prepare the environment for future cybersecurity projects.
# Purpose of the Lab
The purpose of the lab is to establish a controlled and isolated cybersecurity testing environment for developing practical skills in network security, ethical hacking, penetration testing, vulnerability assessment and cybersecurity troubleshooting. The lab uses VirtualBox and Kali Linux as the foundation, with a dedicated 10.0.0.0/24 NAT Network. This laboratory provides a safe environment to practice cybersecurity techniques, test security tools, document findings, troubleshoot technical issues, and build practical experience without impacting production systems or unauthorised networks.
# Lab Architecture
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/Lab.png)
# Lab Configuration
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/Lab%20Configuration.png)
# Lab Setup Procedure
# Step 1. Install 7-Zip
7-Zip was installed to extract the Kali Linux virtual machine package, which may be distributed as a .7z archive. 
Tool: 7-Zip
# Step 2. Install VirtualBox
Oracle VirtualBox was installed as the hypervisor.
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/VirtualBox%20.png)
# Step 3. Create the NAT Network
A dedicated NAT Network was created in Oracle VirtualBox.
Configuration: Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Yes IPv6: No
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/NAT%20Configuration.png)
# Step 4. Import Kali Linux
The Kali Linux virtual machine was downloaded from the official Kali Linux website and imported into VirtualBox.
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/Kali%20Linux.png)
# Step 5. Configure the Kali Linux Network
The Kali Linux network configuration was checked and configured with a consistent IPv4 address.
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/Static%20IP%20Configuration.png)
# Step 6. Create a Clean VM Snapshot
After completing the initial configuration, a VirtualBox snapshot (Backup) was created.
![image.alt](https://github.com/Eneya-Banda/networkwalks-cybersecurity-lab-setup-v1/blob/main/Snapshot.png)
# Problems Encountered

# Internet Connectivity After Static IP Configuration
After manual configuration of the IPv4 settings, Internet connectivity may fail depending on the Kali/NetworkManager configuration. The command "sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0" sorts out this issue
# What I learned 
Through this lab, I gained practical experience in setting up a basic cybersecurity testing environment using VirtualBox and Kali Linux.
# Learning Outcomes
- How to use VirtualBox to create and manage virtual machines for cybersecurity practice.
- How to configure a NAT Network using the 10.0.0.0/24 subnet.
- How to configure a static IP address for Kali Linux using 10.0.0.2/24 as the required lab address.
- The importance of network configuration when building a cybersecurity lab.
- Configure Kali Linux to maintain Internet connectivity while operating within the virtual lab network.
- The importance of taking virtual machine snapshots before performing further configurations or security experiments.
- Gained a better understanding of how to build a safe and controlled environment for practising ethical hacking and cybersecurity techniques.
# Key Takeaway
The most important lesson from this exercise was that a properly configured and isolated laboratory is the foundation for effective cybersecurity and ethical-hacking practice. Before performing security testing, it is important to establish the network architecture, configure the systems correctly, create recovery points, and ensure that testing is conducted in an authorised environment.
# 1. NAT Vs NAT Network
A NAT Network allows multiple virtual machines to communicate with each other while also providing internet access through network address translation, making it ideal for building a multi-machine cybersecurity lab.
# 2. Virtual Machine Networking
I learned how VirtualBox network adapters connect virtual machines to different network environments and how network settings influence communication between the virtual machines.
# 3. VM Snapshots
I learned the importance of creating a clean snapshot before carrying out risky or experimental activities, providing a reliable recovery point that can be restored during future cybersecurity exercises.
# 4. Documentation
I learned that keeping clear records of commands, configurations, screenshots, challenges, and their solutions is essential for maintaining a professional cybersecurity project.
# 5. Static IP Configuration
I learned how to configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in Kali Linux.
# 6. Documentation
I learned that documenting commands, configuration, screenshots, problems, and solutions is an important part of a professional cybersecurity project.
# Security and Ethical Use
This laboratory is intended strictly for educational purposes only.
# Tools and Resources
- 7-Zip: https://7-zip.org/download.html
- VirtualBox: https://virtualbox.org/wiki/Downloads
- Kali Linux: https://kali.org/get-kali
# Author
Eneya Joseph Banda | Cybersecurity Professional B083 | LinkedIn: https://www.linkedin.com/in/eneya-joseph-banda-78325262/
# Project Information
Program Name: Cybersecurity at Networkwalks | Week: 01 | Project: Cybersecurity & Pentesting Lab Setup | Repository: GitHub





