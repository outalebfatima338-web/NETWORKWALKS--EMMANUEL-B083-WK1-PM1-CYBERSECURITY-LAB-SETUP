# NETWORKWALKS--EMMANUEL-B083-WK1-PM1-CYBERSECURITY-LAB-SETUP
📌 Project Overview

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.

The purpose of this lab is to create a controlled environment where cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities can be performed safely and repeatedly.

The lab is configured on a private virtual network so that additional machines can be added later and used as targets for authorized security testing.

 Objectives

-The main objectives of this project are to:

-Install and configure VirtualBox.

-Install/import Kali Linux as a virtual machine.

-Create a private NAT Network for the cybersecurity lab.

-Configure network connectivity for Kali Linux.

-Assign a consistent IP address to the Kali VM.

-Configure the default gateway and DNS server.

-Verify network connectivity and DNS resolution.

-Take a clean VM snapshot for recovery.

-Document the complete setup process.


🛠️ Tools and Technologies

-VirtualBox 7.2
-Kali Linux 2026.2
-Windows 11
-NAT Network
-Linux Terminal

🛡️ Purpose of the Lab
The lab provides an isolated and controlled environment for cybersecurity learning and authorized security testing.

It can be used for activities such as:

Network reconnaissance
-Port scanning
-Vulnerability assessment
-Packet analysis
-Web security testing
-Exploitation practice
-Security-tool experimentation

 ⚙️ Lab Configuration

|  Component |  Configuration |
|---|---|
| 💻 Host OS | Windows 11 |
| 🧠 Host RAM | 8 GB |
| ⚡ Processor | Intel Core i8 |
| 🧰 Hypervisor | VirtualBox 7.2 |
| 🐉 Security OS | Kali Linux |
| 🧠 Kali RAM | 3048 MB |
| 🌐 Virtual Network | NAT Network |
| 📡 Network Address | 10.0.0.0/24 |
| 🖥️ Kali IP Address | 10.0.0.2 |
| 🚪 Default Gateway | 10.0.0.1 |
| 🌍 DNS Server | 8.8.8.8 |

🔎 Lab Verification
|✅ Test|	🧾 Command	|🎯 Expected Result|
|🌐 Check IP address|	ip a	|Correct Kali IP displayed|
|📡 Test gateway|	ping 10.0.0.1|	Successful replies|
|🌍 Test Internet connectivity|	ping 8.8.8.8|	Successful replies|
|🔎 Test DNS resolution	nslookup| networkwalks.com|	Domain resolves|
|🧰 Verify Nmap|	nmap --version	|Nmap version displayed|
|🔄 Verify snapshot|	Restore snapshot and run ip a	|Baseline configuration restored|


💡 What I Learned
Through this project, I learned how to create and configure a virtual environment for cybersecurity practice.

The most important concepts I learned include:

1. NAT vs NAT Network
A standard NAT configuration and a NAT Network serve different purposes.

A NAT Network allows multiple VMs connected to the same virtual network to communicate with one another while providing network address translation for external connectivity.

This makes it useful for building a multi-machine cybersecurity laboratory.

2. Virtual Machine Networking
I learned how VirtualBox virtual network adapters connect virtual machines to different types of networks and how network configuration affects communication between machines.

3. Static IP Configuration
I learned how to configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in Kali Linux.

4. VM Snapshots
I learned that a clean snapshot should be created before performing risky or experimental activities.

This provides a known-good recovery point for future cybersecurity exercises.
