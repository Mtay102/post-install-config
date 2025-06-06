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

- Windows 10<br>

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles (for grouping permissions)
- Configure Departments
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics

<br>

<p>
Admin/Analyst Login Page:<br>
http://localhost/osTicket/scp/login.php 
<br>
<br>
End Users osTicket URL:<br>
http://localhost/osTicket 
</p>

<h2>Configuration Steps</h2>

<p>
Configure Roles (for grouping permissions)<br>
Admin Panel -> Agents -> Roles<br>
  - Add new role (Supreme Admin)
</p>

![ost1](https://github.com/user-attachments/assets/aaaacf91-324f-4260-b3ed-b1a97c0fe92a)

<br>

<p>
Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)<br>
Admin Panel -> Agents -> Departments<br>
  - SysAdmins
</p>

![ost2](https://github.com/user-attachments/assets/40842010-1892-4f59-a906-11d2a744f730)

<br>

<p>
Configure Teams<br>
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)<br>
  - Online Banking
</p>

![ost3](https://github.com/user-attachments/assets/f2bf0407-9851-4fc9-b762-eb3e8ebfb232)

<br>

<p>
Allow anyone to create tickets<br>
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)<br>
  - Registration Required: Require registration and login to create tickets 
</p>

<br>

<p>
Configure Agents (workers)<br>
Admin Panel -> Agents -> Add New<br>
  - Jane (Dept: SysAdmins)<br>
  - John (Dept: Support)
</p>

![ost4](https://github.com/user-attachments/assets/1d2d1010-4b69-4ff2-b9ff-8d1c60df96ff)

<br>

<p>
Configure Users (customers)<br>
Agent Panel -> Users -> Add New<br>
  - Karen<br>
  - Ken
</p>

img 

<br>


<p>
Configure SLA<br>
Admin Panel -> Manage -> SLA<br>
  - Sev-A (Grace Period: 1 hour, Schedule: 24/7)<br>
  - Sev-B (Grace Period: 4 hours, Schedule: 24/7)<br>
  - Sev-C (Grace Period: 8 hours, Business Hours)
</p>

img 

<br>


<p>
Configure Help Topics (For when users create a ticket)<br>
Admin Panel -> Manage -> Help Topics<br>
  - Business Critical Outage<br>
  - Personal Computer Issues<br>
  - Equipment Request<br>
  - Password Reset<br>
  - Other
</p>

img 
