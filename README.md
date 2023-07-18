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

- Ensure connectivity between the two  Virtual machines and install Active Directory 
- Create an Admin/Normal user account in Active Directory 
- Setup Virtual machines for non-administrative user and create addtions user
  

<h2>Deployment and Configuration Steps</h2>

<p>
<a href="https://imgur.com/ZsVisEN"><img src="https://i.imgur.com/ZsVisEN.png" title="source: imgur.com" /></a>
<a href="https://imgur.com/sXhmKCD"><img src="https://i.imgur.com/sXhmKCD.png" title="source: imgur.com" /></a>
</p>
<p>
Firstly, we will login into client-1 of our remote desktop and ping the secound Virtual Machine(DC-1's) private IP. Generating a Perpetual ping and enable ICMPv4 in fire wall of DC-1(Domain Controller), logining back in ans install Active Directory Domain Services. Setting up a new forset ans restart and log back into DC-1. 
</p>
<br />

<p>
<a href="https://imgur.com/C0cAv9r"><img src="https://i.imgur.com/C0cAv9r.png" title="source: imgur.com" /></a>
<a href="https://imgur.com/VzXjgJb"><img src="https://i.imgur.com/VzXjgJb.png" title="source: imgur.com" /></a>
</p>
<p>
Afterwards, in Active Directory users and computers we'll create organizaton units. Setting up the DNS settings for Client-1 through the Azure portal, logining back in with the admin user(labuser) as before. 
</p>
<br />

<p>
<a href="https://imgur.com/4kU81SL"><img src="https://i.imgur.com/4kU81SL.png" title="source: imgur.com" /></a>
</p>
<p>
Lastly we will setup remote desktop for Non-administrative user, additionally creating more users and attempt to log into client-1 as one of the user. 
</p>
<br />
