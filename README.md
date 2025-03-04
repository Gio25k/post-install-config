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

- Login to the osTicket admin Panel
- Configure Roles
- Configure Departments
- Configure Teams
- Configure Help Topics

<h2>Configuration Steps</h2>

<p>
  Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access. An unlimited number of roles can be created and assigned to Agents with access to various departments.
Admin Panel -> Agents -> Roles
Supreme Admin
<img src="https://i.gyazo.com/a926cfe925584288f523c94269713dd0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.gyazo.com/9df04eae5906630e19349c0556eb6b1e.png="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enter "Supreme Admin" as the role and enable every possible permission available
</p>
<br />

<p>
<img src="https://i.gyazo.com/5ce87fe2224e3d4a4dfa5934748ab6c8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department.
Admin Panel -> Agents -> Departments
SysAdmins
Leave the remaining fields set as default and simply review what selections are available to choose from

</p>


<p>
<img src="https://i.gyazo.com/c3b5099a4bb3ff3730657f6aac955031.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.gyazo.com/97940eaa165c85ba8eb9171db132e477.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter.
Admin Panel -> Agents -> Teams -> Add new Team named Online Banking


</p>
<br />

<p>
<img src="https://i.gyazo.com/b4875844b6347ab2986d8afa3f4a36db.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<br />

<p>
<img src="https://i.gyazo.com/68052b0c0d2e16fcbb7a473b2000ee25.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
Registration can be required for Users to create tickets on the Help Desk to prevent random tickets or to limit Users’ accessibility to the help desk.
Admin Panel -> Settings -> User Settings
Registration Required: Require registration and login to create tickets -for this lab, we will leave it unchecked so that tickets can be created without restrictions/limitations
<p>
<img src="https://i.gyazo.com/56e44052fa879dc056907f0fec8aea0f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent’s Profile.
Admin Panel -> Agents -> Add New
Jane
John

<p>
<img src="https://i.gyazo.com/6524a1c3c416fd5dcfeb9090b455b43e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


<p>
<img src="https://i.gyazo.com/d4d788e80a63a52ab2276f3cf28ddd87.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Users (customers) can create an account and log in to create a ticket or check on their ticket status as well.
Agent Panel -> Users -> Add New
Karen

<p>
<img src="https://i.gyazo.com/29b613005b210ac24073a72003057599.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Now we will add SLA Plans
<p>
<img src="https://i.gyazo.com/2d992d680266391d83495ae3de399382.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed. Admin Panel -> Manage -> SLA
Sev-A (1 hour, 24/7)
Sev-B (4 hours, 24/7)
Sev-C (8 hours, business hours)
  Be sure to add all 3 SLA Plans.
</p>
<br />
<p>
<img src="https://i.gyazo.com/55f04bfc3aac5fec785dc9427e946e50.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
And in the end it should look like this
</p>
<br />

<p>
<img src="https://i.gyazo.com/a60f5919273c84f7aa92af8c898c34a1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for further breakdown (For example, Human Resources and Human Resources/Payroll.)
Admin Panel -> Manage -> Help Topics
Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset
</p>
<br />

<p>
<img src="https://i.gyazo.com/7480f91f2394a978cf6190b7d2dc5a50.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />
<p>
<img src="https://i.gyazo.com/15e25a918be11ed61223151b84de1ad7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


<p>
<img src="https://i.gyazo.com/3ed12e0743a605c00c08da2584853d95.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<p>
<img src="https://i.gyazo.com/64064d0d29b10ac5a80bd9d2de65c008.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<br />
<img src="https://i.gyazo.com/cabf5fbd2d9bcbf8d30cbedd743412ca.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
