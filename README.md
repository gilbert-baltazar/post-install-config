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

<img width="1682" alt="Screen Shot 2024-05-19 at 11 33 31 AM" src="https://github.com/DereHz/post-install-config/assets/169094076/c92ed798-f69c-4cff-aabf-019666231ec2">

Step 1. Configure Roles
 - Admin Panel -> Agents -> Roles -> Add New role
 - Add a name
 - Click "Permissions" and Check all boxes on Tickets\Tasks\Knowledgebase
 - Click Add Role


<img width="1686" alt="Screen Shot 2024-05-19 at 11 42 01 AM" src="https://github.com/DereHz/post-install-config/assets/169094076/61440146-9d35-41f2-943a-c03e9dc521f1">

Step 2. Configure Departments 
 - Admin Panel -> Agents -> Departments
 - Click "Add New Department"
 - Name it System Administrators


<img width="1683" alt="Screen Shot 2024-05-19 at 11 50 22 AM" src="https://github.com/DereHz/post-install-config/assets/169094076/34509ae3-6de3-4f79-bed3-1ba2259ee902">

Step 3. Configure Teams
 - Admin Panel -> Agents -> Teams
 - Click on "Add new Team"
 - Name it "Level II Support"

Note: There should be a "Level I Support" team already there

<img width="1684" alt="Screen Shot 2024-05-19 at 11 58 21 AM" src="https://github.com/DereHz/post-install-config/assets/169094076/5ed0b17a-d3e4-469d-91fc-183460339c24">


Step 4. Allow anyone to create tickets 
 - Admin Panel -> Settings -> User Settings
 - Make sure the "require registration and login to create tickets" box is unchecked

<img width="1682" alt="Screen Shot 2024-05-19 at 12 10 45 PM" src="https://github.com/DereHz/post-install-config/assets/169094076/15ec0dc3-134f-4465-a6cc-3203d48d7220">

Step 5. Configure Agents (Workers)
 - Admin Panel -> Agents -> Add New Agent
 - Jane Doe - username: Jane.doe, "Access" System Administrators and Superb Admin, "Teams" put on Team II
 - John Doe - username: John.doe, "Access" Support, View only


<img width="1682" alt="Screen Shot 2024-05-19 at 12 16 54 PM" src="https://github.com/DereHz/post-install-config/assets/169094076/0ef92a6d-851a-418f-9961-0f7d961090c6">

Step 6. Configure Users (Customers) 
 - Agent Panel -> Users -> Add New
 - Sarah Doe
 - Ken Doe


<img width="1629" alt="Screen Shot 2024-05-19 at 12 23 22 PM" src="https://github.com/DereHz/post-install-config/assets/169094076/b200f14d-86f1-471a-a516-f542acb5308e">


Step 7. Configure SLA
 - Admin Panel -> Manage -> SLA
 - Sev-A (1 hour, 24/7)
 - Sev-B (4 Hours, 24/7)
 - Sev-C (8 hours, Business Hours)


<img width="1639" alt="Screen Shot 2024-05-19 at 12 31 22 PM" src="https://github.com/DereHz/post-install-config/assets/169094076/671446f1-57d7-487c-a16d-731f0bcc6392">

Step 8. Configure Help Topics
 - Admin Panel -> Manage -> Help Topics
 - Business Critical Outage
 - Personal Computer Issues
 - Password Reset 

