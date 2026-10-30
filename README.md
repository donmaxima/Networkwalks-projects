Project Overview:

This project focuses on setting up a virtual cybersecurity and penetration-testing laboratory using VirtualBox and Kali Linux.
The lab provides a controlled environment to safely and repeatedly practice cybersecurity tools, network scanning, reconnaissance, vulnerability assessment, and other security-testing activities.
Main Objectives:

Install and configure VirtualBox.
Install/import Kali Linux as a virtual machine.
Create a private NAT Network for the cybersecurity lab
Configure network connectivity for Kali Linux.
Assign a consistent IP address to the Kali VM.
Verify network connectivity and DNS resolution.
Take a clean VM snapshot for recovery.
Purpose of the Lab:

The lab provides an isolated and controlled environment for learning in cybersecurity and approved security testing such as:
Network reconnaissance
Port scanning
Vulnerability assessment
Packet analysis
Web security testing
Exploitation practice
Security-tool experimentation
Procedures:

1.	Download and install Oracle VirtualBox
2.	A dedicated NAT Network was created in VirtualBox.
3.	Configuration: Network Name: NatNetwork IPv4 Prefix: 10.0.0.0/24 DHCP: Enabled IPv6: Disabled .<img width="1920" height="1280" alt="Screenshot 2026-10-30 211757" src="https://github.com/user-attachments/assets/5e12365d-be9e-45e1-a78c-3095971faed4" />
4.	Import the Kali Linux virtual machine into VirtualBox. <img width="1916" height="1278" alt="Screenshot 2026-10-30 210714" src="https://github.com/user-attachments/assets/61c72171-e098-45fd-b927-ddc5cf55ee30" />

5.	Configure the Kali Linux Network: The Kali Linux network configuration was checked and configured with a consistent IPv4 address. <img width="1915" height="1280" alt="Screenshot 2026-10-30 210829" src="https://github.com/user-attachments/assets/d4477170-010d-42da-8ec1-b3dbb3323a30" />



Problems Encountered & Solutions:

Internet Connectivity After Static IP Configuration
After manually configuring the IPv4 settings, Internet connectivity failed 
One workaround used during this lab was changing my DNS settings from 8.8.8.8 to 10.0.0.1
What I Learned
Through this project, I learned how to create and configure a virtual environment for cybersecurity practice.

The most important concepts I learned include:

1. NAT vs NAT Network
A standard NAT configuration and a NAT Network serve different purposes.
A NAT Network lets multiple VMs on the same virtual network communicate with one another while providing network address translation for external connectivity. This makes it useful for building a multi-machine cybersecurity laboratory.
2. Virtual Machine Networking
I learned how VirtualBox virtual network adapters connect virtual machines to different types of networks and how network configuration affects communication between machines.
3. Static IP Configuration
I learned how to configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in Kali Linux.
4. VM Snapshots
I learned that a clean snapshot should be created before performing risky or experimental activities.
This provides a known-good recovery point for future cybersecurity exercises.

