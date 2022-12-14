<p align="center">
<img src="https://i.imgur.com/yMBdniV.png" alt="Microsoft Active Directory Logo"/>
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

- Create DC-1 and Client-1 virtual machines (both windows Server)
- Copy virtual ip address and remote connect
- Add roles on server manager
- Install Active Directory

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/MDjxkvm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created both DC-1 and Client-1 VMs.



<p>
<img src="https://i.imgur.com/c4vYcQa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Went to DC-1 in Azure and clicked on the NIC >Ip Configuration > Changed the IP Address from Dynamic to Static in order for the IP adress to not change.

<p>
<img src="https://i.imgur.com/UedV58O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Adding roles and features. Installing Active Directory Domain Services in the server manager in DC-1.
  
<p>
<img src="https://i.imgur.com/7IqEf62.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created "mydomain.com" then installed Active Directory Services. DC-1 VM restarted. Then searched "Active Directory Users and Computers" and Active Directory is successfully installed!
