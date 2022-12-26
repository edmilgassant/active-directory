<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create virtual machine (Windows Server)
- Copy virtual ip address and remote connect
- Add roles on server manager
- Install Active Directory

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/Z845RBh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Doing a configuration on a virtual machine under DC-1 to static instead of dynamic. Static means the IP address won't change if I turned off the computer or if it shuts down or anything, it will remian the same. 
</p>
<br />

<p>
<img src="https://i.imgur.com/vmme7IE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created two VM's and going to make sure they both are receiving, acknowledging and replying within the same virtual network using ICMPv4. DC-1 is Windows version. Client-1 is Ubuntu version.

<p>
<img src="https://i.imgur.com/7unkGzh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Adding roles and features. Installing Active Directory Domain Services in the server manager in DC-1. Going to allow the ICMPv4 versions.
