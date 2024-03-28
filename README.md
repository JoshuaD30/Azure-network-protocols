<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://youtu.be/gzbTm5r5Fv8)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create a DNS A-Record in DC (Domain Controller)
- Create a CNAME record, and observe changes with ping "search", nslookup, ipconfig, and other commands.
- Create file shares "read-access", "write-access", "no-access", "accounting" with various permissions. Attempt to access file shares as a normal user.
- Create an "ACCOUNTANTS" (Security Group) in Active Directory, and assign permissions to test access.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/SX1W5Nh.png" height="80%" width="80%" alt="A-Record"/>
</p>
<p>
A-Record in DC (Domain Controller).
</p>
<br />

<p>
<img src="https://i.imgur.com/20q4JrA.png" height="80%" width="80%" alt="Local DNS Cache"/>
</p>
<p>
Checking the local DNS after chaning the ip address to 8.8.8.8.
</p>
<br />

<p>
<img src="https://i.imgur.com/FJXxtpP.png" height="80%" width="80%" alt="CNAME"/>
</p>
<p>
CNAME record created and now pinging it.
</p>
<br />

<p>
<img src="https://i.imgur.com/dtjXMPK.png" height="80%" width="80%" alt="permissions for each folder"/>
</p>
<p>
File shares "read-access", "write-access", "no-access", "accounting" created with permissions.
</p>
<br />
