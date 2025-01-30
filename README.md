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

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
