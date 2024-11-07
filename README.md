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

- Windows 10 Pro (22H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure SLAs
- Configure Help Topics

<h2>Configuration Steps</h2>
<p>
In this lab, we will be using both the admin portal and end user portal:</p>

- Admin/Analyst Login Page:
http://localhost/osTicket/scp/login.php 

- End Users osTicket URL:
http://localhost/osTicket 

Our admin portal should look like this:

![image](https://github.com/user-attachments/assets/4a56dd1f-ae93-4a81-a368-cdabf979e338)

Followed by an Open ticket with the subject( osTicket Installed!):

![image](https://github.com/user-attachments/assets/a906de3a-fc7c-4ea3-be62-f76a1df7eb20)

<p>Log in to your admin account with the credentials you entered previously the first time you installed osTicket.</p>

![image](https://github.com/user-attachments/assets/d92102cc-6eb1-4748-9647-52b3039df655)
![image](https://github.com/user-attachments/assets/0e762d13-48a4-46be-95ba-47e8d12b0d27)







<h3>Configure Roles</h3>
<p>First, head to the Agents tab > Roles > Add New Role</p>
<p>Here we will create a Supreme Admin who will have full access and permissions privileges</p>
<p>Check all the boxes under the Permissions tab, in the Tickets/Tasks/Knowledgebase sub-tabs.</p>
We can name this role "Supreme Admin"

![image](https://github.com/user-attachments/assets/c31ea18f-7019-452c-bc4d-bdc1eb1d102f)
![image](https://github.com/user-attachments/assets/ae921faa-e918-49c8-a551-e3f690d392a6)
![image](https://github.com/user-attachments/assets/3d0dcca9-d007-48e9-81a2-865b5e780d2e)
![image](https://github.com/user-attachments/assets/3614b95f-f867-4757-b2f0-01f910e2a4d8)
![image](https://github.com/user-attachments/assets/f0aa3547-7283-48e1-8847-3454d5cc9346)





<br />
<h3>Configure Departments</h3>
<p>Next, we can add some departments to our enterprise. Let's create one called "SysAdmin"</p>
<p>Navigate to the Agents tab > Departments > Add New Department</p>
<p>Parent: Top Level Deparment</p>
<p>Name: SysAdmins</p>
<p>Access: Agents who have extended access to this department have not yet been added to the system yet</p>


![image](https://github.com/user-attachments/assets/19641b1b-e7ab-4e91-9f90-8bb3887f14cd)
![image](https://github.com/user-attachments/assets/6f8a6c0d-6c1c-4b14-bcf9-c152389f34e7)
![image](https://github.com/user-attachments/assets/0031e072-3ab4-4941-af4d-e123f9ce0783)





<h3>Configure Teams</h3>
<p>Here, we can create a team called "Online Banking"</p>
<p>In this example, a team may be working on a specific ticket. A team of individuals working on a ticket may be necessary depending on the severity of the ticket submitted.</p>
<p>Navigate to the Agents tab > Teams </p>
<p>We will add a new team titled "Online Banking"</p>

![image](https://github.com/user-attachments/assets/5cffa9d6-1a1c-4914-bd2a-b5662cb29972)
![image](https://github.com/user-attachments/assets/9a9e270e-f8d4-4773-ad30-6a8eeb1d89b2)




<h3>Configure Agents and Users</h3>
<p>Let's add some agents!</p>
<p>Navigate to Agents tab > Agents > Add New Agent</p>
<p>If you see your Name: Marvin Sanchez and Username: admin1, you clicked on the right tab</p>
<p>We can create an agent who may work in the support department and another who works in the SysAdmin department</p>
<p>We can add a non-existent email such as janedoe@example.com</p>
<p>Make sure you note your agent's username. For example: agent Jane Doe may have username: janedoe</p>
<p>We also need to set a password to log in as our agent. Make sure you click "set password" > uncheck the box "Send the agent a password reset email" > click "set" >  set a password like "Password1" (and make sure you make note of it) > and uncheck the box "Require password change at next login"</p>

![image](https://github.com/user-attachments/assets/1d17df9e-bf3c-4a89-9bde-cb01056afb02)


<p>Agent#1: Jane Doe!</p>
<p>Agent will have extensive access and will be assigned to Team: Online Banking </p>

![image](https://github.com/user-attachments/assets/b17bb913-1e2d-4a3b-bae2-773f3fa998f7)
![image](https://github.com/user-attachments/assets/2d911e53-c028-408c-980c-d519f6a8e6e2)
![image](https://github.com/user-attachments/assets/6948c666-ee9e-40f6-a81e-37d87dfbf779)

<p> Agent#2: John Doe!</p>
<p> Agent will have limited access</p>

![image](https://github.com/user-attachments/assets/d960d4c4-f918-4cff-9472-7e5cf0f806cc)
![image](https://github.com/user-attachments/assets/7111799e-d2ea-4b99-8929-96547e323236)


<p> User: Karen</p>
<p> Switch over to Agent Panel</p>

![image](https://github.com/user-attachments/assets/a57b7f98-754e-4b48-9176-fff42425e20d)
![image](https://github.com/user-attachments/assets/c0ab0547-6d2c-4715-bda6-8554d1b35152)
![image](https://github.com/user-attachments/assets/c059c9dd-d6fc-4e70-a1a0-f9704ff62849)








<h3>Configure SLAs</h3>
<p>Next, we will configure SLAs.</p>
<p>SLAs help manage customer expectations by clearly defining the scope and quality of services to be delivered. In a ticketing system, SLAs are crucial as it sets clear expectations regarding service delivery, such as response time, uptime guarantees, and resolution times for customer support issues.</p>
<p></p>We can create three SLAs of varying severities titled "Sev-A"; "Sev-B"; and "Sev-C"</p>
<p>Navigate to the Manage tab > SLA > "Add New SLA Plan"</p>

- Sev-A: Grace Period: 1 hour; Schedule: 24/7
- Sev-B: Grace Period: 4 hours; Schedule: 24/7
- Sev-C: Grace Period: 8 hours; Schedule: Monday - Friday with U.S. Holidays

<p>These schedules can be changed as well. You can play around with the schedules and add your own under the Manage tab > Schedules</p>

![image](https://github.com/user-attachments/assets/4ef34d2c-88c8-4df7-b066-11aed535ffb5)
![image](https://github.com/user-attachments/assets/14b6bc04-6a86-4955-8a53-ae84c16507d2)
![image](https://github.com/user-attachments/assets/fdc5421f-f51a-400b-b1e3-7fde8cfc67a9)
![image](https://github.com/user-attachments/assets/5e334741-2b24-40f0-bc44-18a08665f76a)



<h3>Configure Help Topics</h3>
<p>A help topic in a support ticket system is a categorized subject that provides users with guidance, resources, and solutions related to specific issues or inquiries they may encounter.</p>
<p>Navigate to the Manage tab > Help Topics > Add New Help Topic</p>
<p>We can create one such as "Business Critical Outage" under "Report a Problem"</p>
And another such as "Personal PC Issues"

![image](https://github.com/user-attachments/assets/ae2890a7-f669-4a54-8144-f96c2a495c7a)
![image](https://github.com/user-attachments/assets/054d15c3-2147-4305-a0e2-85b113b0d3a0)
![image](https://github.com/user-attachments/assets/dd0e16c5-49cc-4e60-a05b-244d742ca6ed)
![image](https://github.com/user-attachments/assets/0d2453a8-80df-478e-ac47-6423ccebaed5)
![image](https://github.com/user-attachments/assets/546835d1-b3bf-4b34-b4a4-3e0080dfb990)
![image](https://github.com/user-attachments/assets/2c4129a2-be65-41e6-aab3-777df0efa3b7)
![image](https://github.com/user-attachments/assets/4a8fb6c4-015c-468b-8756-f6a7004cb755)






<p>We are finished with the post-installation configuration! In the next tutorial, we will go through working sample tickets.</p>

