<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
Hey there! This is a guide on how to configure osTicket, an open-source help desk ticketing system, after the installation process.<br />

<b>Note:</b> To follow along with this guide, make sure you have completed the prerequisites and installation steps described in my previous demonstration, "Prerequisites and Installation".

<h2>Video Demonstration</h2>

- ### [How To Configure osTicket, post-installation](https://drive.google.com/file/d/1dFvXN6I8EnOFGr2uQspMP-gzzkNG1OoA/view?usp=sharing)

<h2>Environments and Technologies Used</h2>
Microsoft Azure (Virtual Machines/Compute)
Remote Desktop
Internet Information Services (IIS)
osTicket Documentation
<h2>Operating Systems Used</h2>
Windows 10 (21H2)
<h2>Post-Install Configuration Objectives</h2>
Let's take a look at the objectives we'll cover during the configuration:

Create and Configure Roles
Create and Configure Departments & Teams
Create and Configure Agents (workers) & Users (clients)
Configure SLA (Service Learning Agreements)
Configure Help Desk Topics
<h2>Configuration Steps</h2>
<h3>&#9312; Prerequisites and Installation</h3>
Before we begin, please ensure that you have set up a virtual machine and installed the prerequisite files for osTicket. You can find the necessary credentials and configurations in the "Prerequisites and Installation" guide. Let's get started!

<hr>
<h3>&#9313; Admin Panel - Roles, Departments, Teams, & Agents</h3>
To begin the configuration, open the Microsoft Edge web browser and navigate to the Help Desk Login Page. Sign in using your osTicket Help Desk credentials (for example, username ostuser / ostuser@email.com).

Help Desk Login Page -- http://localhost/osTicket/scp/login.php
<p align=center>
<img src="https://i.imgur.com/2NAyZo5.jpg" height="100%" width="=100%" alt="Disk Sanitization Steps"/>
</p>
Once you're on the Agent Panel, click on the "Admin Panel" option located at the top-right corner of the page.

<p align=center>
<img src="https://i.imgur.com/dByQbR1.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
In the Admin Panel, go to the "Agents" tab and click on "Roles". Then, select "Add New Role".

<p align=center>
<img src="https://i.imgur.com/mjTZZ5h.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Roles are important as they determine the permissions granted to Agents based on the Departments they have access to. In the Definition tab, enter a name for the Role you want to create (let's use Supreme Admin in this example).

This role will have all permissions.
Next, navigate to the Permissions tab.
<p align=center>
<img src="https://i.imgur.com/U8vxJEe.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Under the Permissions tab, in the Tickets category, make sure to checkmark ALL boxes.

Remember to do the same for the Agent Tasks, Knowledgebase, Dashboard, and Configuration categories as well. This will give the Supreme Admin role full access to all features and functionalities.

Click on "Add Role" to save the new role.

Next, let's create departments and teams. In the Admin Panel, go to the "Agents" tab and click on "Departments". Then, select "Add New Department".

In the Department Creation form, provide a name for the department (e.g., "IT Support") and optionally, a description. Click on "Add Department" to save it.

Now, let's create teams within the department. Under the department you just created, click on "Teams". Then, select "Add New Team".

In the Team Creation form, provide a name for the team (e.g., "Level 1 Support") and select the department it belongs to. Click on "Add Team" to save it.

Next, let's create agents (workers) and users (clients). In the Admin Panel, go to the "Agents" tab and click on "Add New Agent".

Fill in the Agent Creation form with the necessary details, including the agent's name, email address, and username. Assign the agent to the appropriate department and team. Set a password for the agent and select the role (e.g., "Supreme Admin") you created earlier. Click on "Create Agent" to save it.

To create users, navigate to the "Users" tab in the Admin Panel and click on "Add New User". Fill in the User Creation form with the required details, including the user's name, email address, and username. Set a password for the user and select the default role for clients. Click on "Create User" to save it.

<h3>&#9314; SLA Configuration</h3>
In the Admin Panel, go to the "Tickets" tab and click on "SLA". Then, select "Add New SLA Plan".

Provide a name for the SLA plan (e.g., "Standard SLA") and configure the various settings, such as response time, resolution time, and escalation rules. Customize the SLA rules based on your organization's requirements. Click on "Create SLA" to save it.

<h3>&#9315; Help Desk Topics Configuration</h3>
In the Admin Panel, go to the "Tickets" tab and click on "Topics". Then, select "Add New Topic".

Provide a name for the topic (e.g., "Technical Support") and optionally, a description. Configure other settings as needed, such as the priority and whether the topic is public or private. Click on "Create Topic" to save it.

That's it! You have successfully completed the post-install configuration steps for osTicket. You can continue customizing and fine-tuning the system based on your organization's specific requirements.

Remember to refer to the official osTicket documentation for more detailed information and guidance.

I hope this helps! Let me know if you have any further questions.
