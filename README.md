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

- Windows 10</b> (22H2)

<h2>Configuration Steps</h2>

![Screenshot 2024-09-03 at 8 25 32 PM](https://github.com/user-attachments/assets/c05243db-8fb7-4e15-b853-280395399d7d)

Step 1. Configure Roles
 - Admin Panel -> Agents -> Roles -> Add New role
 - Add a name
 - Click "Permissions" and Check all boxes on Tickets\Tasks\Knowledgebase
 - Click Add Role


![Screenshot 2024-09-03 at 8 32 00 PM](https://github.com/user-attachments/assets/9cbf0557-4b47-4a99-85f8-8d9de92e76bc)

Step 2. Configure Departments 
 - Admin Panel -> Agents -> Departments
 - Click "Add New Department"
 - Name it System Administrators


![Screenshot 2024-09-03 at 8 32 45 PM](https://github.com/user-attachments/assets/e30f1713-1f21-4c63-a026-a1ceb9c84326)

Step 3. Configure Teams
 - Admin Panel -> Agents -> Teams
 - Click on "Add new Team"
 - Name it "Level II Support"

Note: There should be a "Level I Support" team already there

![Screenshot 2024-09-03 at 8 33 07 PM](https://github.com/user-attachments/assets/7de2bd9a-4e15-41fc-88ba-5e0e7fcdafe3)


Step 4. Allow anyone to create tickets 
 - Admin Panel -> Settings -> User Settings
 - Make sure the "require registration and login to create tickets" box is unchecked

![Screenshot 2024-09-03 at 8 43 31 PM](https://github.com/user-attachments/assets/1a44d09d-dc48-4450-bea7-2dd20f00bc02)

Step 5. Configure Agents (Workers)
 - Admin Panel -> Agents -> Add New Agent
 - Jane Doe - username: Jane.doe, "Access" System Administrators and Superb Admin, "Teams" put on Team II
 - James Doe - username: James.doe, "Access" Support, View only


![Screenshot 2024-09-03 at 8 46 09 PM](https://github.com/user-attachments/assets/a8cddb5d-f2db-44da-9348-a1c2519c388e)

Step 6. Configure Users (Customers) 
 - Agent Panel -> Users -> Add New
 - Karen Karen
 - Ken Ken


![Screenshot 2024-09-03 at 8 48 56 PM](https://github.com/user-attachments/assets/4193a12b-362a-4396-8beb-cbe7b23d18a7)


Step 7. Configure SLA
 - Admin Panel -> Manage -> SLA
 - Sev-A (1 hour, 24/7)
 - Sev-B (4 Hours, 24/7)
 - Sev-C (8 hours, Business Hours)


![Screenshot 2024-09-03 at 8 52 16 PM](https://github.com/user-attachments/assets/e9fb2ac8-9c1a-4bb2-a28e-2f6afb98f73f)

Step 8. Configure Help Topics
 - Admin Panel -> Manage -> Help Topics
 - Business Critical Outage
 - Personal Computer Issues
 - Password Reset 

