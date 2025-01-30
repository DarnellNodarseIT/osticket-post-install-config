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
- Go to Admin panel > Agents > Roles (Note!! if on the top right it says "Agent Panel" this means you are in the Admin Panel, if it says "Admin Panel" then you are in the Agent Panel).
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
- Admin Panel -> Settings -> User Settings (Note!! Under "Authentication Settings" make sure you leave "Registration Required" unchecked)
<p>
<img src="https://i.imgur.com/9YXFiCR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>


5.) Configure Agents (workers)



<p>
- Admin Panel -> Agents -> Add New
<p>
<img src="https://i.imgur.com/XN0qA0O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- We're going to be creating two new agent accounts (Jane Doe and John Doe). 
<p>
- For the username simply enter their first name. For their password enter Password1. (Note!! For setting up their passwords click on "Set Password" then uncheck the "Send reset email" option and you'll be able to setup their passwords).
<p>
- For Jane's Access settings the "Primary Department" will be "Support/SysAdmins" with "Supreme Admin" access.
<p>
- For John's Access settings the "Primary Department" will be "Support" with "View Only" access.
<p>
<img src="https://i.imgur.com/5CZQp0L.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ILsiTtS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>


6.) Configure Users (customers)


<p>
- Agent Panel -> Users -> Add New
<p>
<img src="https://i.imgur.com/HPzDHna.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- We're going to be adding a user this time. 
<p>
<img src="https://i.imgur.com/gwUJswF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>


7.) Configure SLA


<p>
- Admin Panel -> Manage -> SLA
<p>
<img src="https://i.imgur.com/wrSujvs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Sev-A (Grace Period: 1 hour, Schedule: 24/7)
<p>
<img src="https://i.imgur.com/9AqxCIF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Sev-B (Grace Period: 4 hours, Schedule: 24/7)
<p>
<img src="https://i.imgur.com/ClWM6QP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Sev-C (Grace Period: 8 hours, Business Hours: Mondays - Friday/8:00am - 5:00pm)
<p>
<img src="https://i.imgur.com/FicPx5S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>


8.) Configure Help Topics (For when users create a ticket)


<p>
- Admin Panel -> Manage -> Help Topics
<p>
<img src="https://i.imgur.com/AZvdxQP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
- Business Critical Outage/Report a problem
<p>
- Personal Computer Issues/Report a problem
<p>
- Equipment Request/General Inquiry
<p>
- Password Reset/Report a problem
<p>
- Other/General Inquiry
<p>
<img src="https://i.imgur.com/fKpqzWb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Congratulations! That concludes the post install and configurations for osTicket!
