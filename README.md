<h1> File Integrity Monitor </h1>

 ### [Post Demonstration](https://medium.com/@lmb.walid/integriy-monitor-file-fim-and-hashing-algorithms-6eda8b77dce6)

 <h2>Description</h2>
This project is a simple PowerShell-based File Integrity Monitoring (FIM) system that helps detect unauthorized changes to files. It uses hashing algorithms (SHA-512) to compare current file states against a saved baseline. If any file is created, modified, or deleted, the system alerts the user with real-time notifications.
<br/>
<br/>
<br/>

<p align="center">
System Diagram<br/>
<img src="https://github.com/user-attachments/assets/adc32864-4c7a-464b-819d-4996147bc74f" height="60%" width="60%" alt="System Diagram"/>
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>VMware Workstation</b>

<h2>Environments Used </h2>

- <b>Windows 11</b>(Client1)
- <b>Windows Server 2019</b> (DC)

<h2>Program walk-through:</h2>

<h4>DC (SERVER 2019)</h4>

- External Network: DHCP.<br/>
- Internal Network: A static IP address (172.16.0.1).
<p align="center">
DC Network Interfaces <br/>

<img src="https://github.com/user-attachments/assets/db47a123-2fe6-421c-8ca7-15474b5fdafa" height="80%" width="80%" alt="Disk Sanitization Steps" />
<br/>

- Active Directory Domain Services (AD DS)
<br/>
<p align="center">
Install Active directory domain service <br/>

<img src="https://github.com/user-attachments/assets/a2d88215-c5dd-4bb6-8b23-d4d278612fcd" height="60%" width="80%" alt="Disk Sanitization Steps" />
<br />

- Promote the Server to Domain Controller
  
<p align="center">
Add domain name <br/>
<img src="https://github.com/user-attachments/assets/cd2527f5-064b-47bb-94dd-d17d4377619e" height="60%" width="80%" alt="Disk Sanitization Steps" />
<br />

- RAS/NAT for Internet Access
  
<p align="center">
Add Remote Access <br/>
<img src="https://github.com/user-attachments/assets/69477bed-d082-4ee3-9dfe-d4a858c6685f" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br/>

<p align="center">
Add Routing <br/>
<img src="https://github.com/user-attachments/assets/a22def78-efe5-49a4-b6e9-02772d333b2a" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br />

<p align="center">
Enable Routing and Remote Access <br/>
<img src="https://github.com/user-attachments/assets/96818269-f441-4a16-b601-dbc87105fa1b" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br />

<p align="center">
Network Address Translation (NAT) <br/>
<img src="https://github.com/user-attachments/assets/63efc74b-dd09-46a6-bcb5-74612f1ccc7e" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br />

- Configure DHCP

<p align="center">
DHCP Scope <br/>
<img src="https://github.com/user-attachments/assets/2cbc5aa5-0617-46e0-8a61-9d93428db370" height="60%" width="60%" alt="Disk Sanitization Steps" />
<br />

- Script to generate 1k Users automatically
<p align="center">
Powershell script to create Users automatically <br/>
<img src="https://github.com/user-attachments/assets/c61cb100-f2e0-4be1-85b3-3b21926c9926" height="80%" width="80%" alt="Disk Sanitization Steps" />
<br />

 <h4>Client1(Windows 11) </h4>
- Joing the same domain as DC

<p align="center">
Join the Client to the Domain <br/>
<img src="https://github.com/user-attachments/assets/2bb119f4-eec5-4129-b8b9-1a75cb9ddaf8" height="80%" width="80%" alt="Disk Sanitization Steps" />
<br />
 
