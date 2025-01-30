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

<h2>Configuration Steps</h2>

We are now going make some system configuration to osTicket, since we have configured osTicket from scratch. So the first thing we will do is configure roles within osTicket. Roles are simply the permissions granted to Agents per Department that they have access to. 

In order to do that you will go to the osTicket browser, from there the admin panel > agents > roles. We will go back to the role tap and make sure it is highlighted. Click on "Add New Role" and type the name of the new role which in case would be "Supreme Admin". Now click on permissions, we are going to assign all permissions to this role just for the sake of this lab. Below is how your screen should look after you complete this step.

<p>
  
![image](https://github.com/user-attachments/assets/a9995dd5-05c6-4794-8251-612ff9d5a1cf)

</p>
<p>
Next we will create departments within osTicket. Ticketing systems are usually operated through departments in order to determine which departments has visibility to certain tickets as well as promoting faster resolutions timeframes. 
  
So in order to create a department from the Agents tab you will click on Departments > Add New Department. We will enter "SysAdmins" in the name section and scroll down to the bottom of the page and click "Create Dept".
  
</p>

![image](https://github.com/user-attachments/assets/29755da6-3e6f-4ac3-bf2a-8a69fed2b1e9)

</p>
<p>
Once we have configured a department(s) it's now time to create to establish a team. Teams allow you to pull Agents from different Departments and organize them to handle a specific issue. We will also check to make sure that users have permissions to create tickets even if they're not registered in the system yet.

From the Agents tab > Teams and in the name section we will type in "Online Banking", then at the bottom of the page click on "Create Team." We will now make sure all users unregistered have perissions to create tickets. From the Admin panel > Settings > Users and just make sure under "Authentication Settings" that the box next to "Registration Required" is unchecked.

</p>

![image](https://github.com/user-attachments/assets/7c7611ad-d5fe-4dfd-8170-2cfe51acc0bf)
</p>
<p>

![image](https://github.com/user-attachments/assets/66bae88b-5728-497a-bfae-22fc3922ed81)

Now it's time to create Agents. Agents are the ones that are given access to the help desk with the intent to respond and resolve the tickets. Agents are assgined to a primary department and given a role for the tickets/tasks routed to that department.

To create and congfigure a new agent within osTicket, we will first go to the admin panel page from there Agents > Add New. On this page we will fill out all the necessary information for the agent and also navigate to the tabs as follows and configure them as well which are, access, permissions, and teams.

</p>

![image](https://github.com/user-attachments/assets/754fb5e6-9c4b-4946-adaf-973647ae7998)

Next we will create a user in osTicket. Users are the ticket owners of the tickets in the help desk. The user is associated with their email address. To create a user go to Agent Panel > Users > Add New.

</p>

![image](https://github.com/user-attachments/assets/8d499319-f7cf-42ad-a16c-10863b7cb509)

We will now create an SLA Plan(Service Level Agreement). The purpose of an SLA plan is to provide a length of time in which the help desk is expected to take a ticket solve it and  close it.

To create an SLA follow these steps, navigate to admin panel > Manage > SLA. Then we will click on "Add New SLA Plan". We will then fill out all the necessary information on that page. Below I have an example of an SLA, where the name is Sev-B, the grace period is 4 hours, and the schedule is 24/7.
