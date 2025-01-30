<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Configure Teams
- Allow anyone to create tickets
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)

<h2>Configuration Steps</h2>

<p>

  
1.) Configure roles (for grouping permissions)


<p> 
- Go to Admin panel > Agents > Roles (Note if on the top right it says "Agent Panel" this means you are in the Admin Panel, if it says "Admin Panel" then you are in the Agent Panel).
<p>
<img src="https://i.imgur.com/OXzVm0k.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Create a new role called Supreme Admin and give it access to everything.
<p>
<img src="https://i.imgur.com/LrwCKlV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

  
2.) Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)


<p>
- Go to Admin Panel > Agents > Departments
<p>
<img src="https://i.imgur.com/jSJMZ9B.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Here all we're going to do is name the new department "SysAdmins", leave everything else as is, then click "Create Dept" at the bottom of the page.
<p>
<img src="https://i.imgur.com/0tWEZOx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

  
3.) Configure Teams


<p>


- Go to Admin Panel > Agents > Teams
<p>
<img src="https://i.imgur.com/JvkMHgw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Here we're doing the same thing we did for Departments. Create a new team called "Online Banking" and leave the rest as is.
<p>
<img src="https://i.imgur.com/WuyT2AG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>


4.) Allow anyone to create tickets


<p>
- Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
<p>




