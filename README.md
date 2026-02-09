<p align="center">
<img width="5120" height="560" alt="xbanner_osTicket-5120x560w jpg pagespeed ic VHDbUulfIn copy" src="https://github.com/user-attachments/assets/46591c77-d0ac-4a66-bc70-b35db5bc511a" />
</p>

<h1>osTicket -  Post-Install Configuration</h1>
Part 2 of a three-part osTicket Install/Configuration/Ticket-Creation tutorial series. Part 2 outlines the post-install configuration of the open-source helpdesk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Azure
- Virtual Machine
- osTicket 


<h2>Good Things to Know</h2>

 - Click on specific positions for a better understanding!
 	- [Roles](https://docs.osticket.com/en/latest/Admin/Agents/Roles.html)
	- [Departments](https://docs.osticket.com/en/latest/Admin/Agents/Departments.html)
	- [Teams](https://docs.osticket.com/en/latest/Admin/Agents/Teams.html) 
	- [Agents](https://docs.osticket.com/en/latest/Admin/Agents/Agents.html)
	- [Users](https://docs.osticket.com/en/latest/Agent/Users/User%20Directory.html).
	- [Service Level Agreement(SLA)](https://docs.osticket.com/en/latest/Admin/Manage/SLA%20Plans.html)
	
   

<h2>Installation Steps</h2>

<h3>Step 1: Open osTicket and Log In

- Log in to osTicket using the credentials you made during the installation tutorial </h3>
	- If you need help installing osTicket, please see my tutorial [here](https://github.com/RoslyndWilliams/osTicket--Prerequisites-and-Installation)

<p align="center">
<img width="80%" height="80%" alt="68747470733a2f2f692e696d6775722e636f6d2f67415856424f322e706e67 copy" src="https://github.com/user-attachments/assets/19d1a790-6286-43ef-8c25-4c235e585ecb" />


<h3>Step 2: Configure Roles </h3>

- Make sure you are in the Admin panel (check the top-right of the screen to see which panel you are in)
	- If it says "Agent," you are in the Admin panel
- Select the Agent tab > Roles > Add New Role
	- Name: Supreme Admin
	- Select Permissions tab and check every box under the "Tickets," "Tasks," and "Knowledgebase" sections
- Select Add Role
	
<p align="center">
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f3974694f4f4e322e706e67 copy" src="https://github.com/user-attachments/assets/d39995ad-c0ba-4853-8638-0e61bd4e3daf" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f4366437a52526b2e706e67 copy" src="https://github.com/user-attachments/assets/7e4d0941-fd83-43fe-a4d9-624d536fff6c" />
</p>


<h3>Step 3: Configure Departments</h3>

- Ensure you are still in the Admin panel
- Select the Agent tab > Departments > Add New Department 
	- Name: System Administrators
- Select Create Department 


<p align="center">
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f663275456c6f4c2e706e67 copy" src="https://github.com/user-attachments/assets/68e913fd-eb97-470d-a7b6-76f9c2d0d1ca" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f58326458776a592e706e67 copy" src="https://github.com/user-attachments/assets/26a03866-5bcf-425c-91ef-b3cfa7c04883" />
</p>


<h3>Step 4: Configure Teams
</h3>

- Select the Agent tab > Teams > Add New Team
	- Name: Level II Support 
- Go to the Members tab and select yourself in "Select Agent" dropdown menu
- Select Create Team
	
<p align="center">
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f76367a7a4e334e2e706e67 copy" src="https://github.com/user-attachments/assets/e3d1ae8c-3b61-4ac6-9948-80f4281a7814" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f344969655338302e706e67 copy" src="https://github.com/user-attachments/assets/6704bec1-d90d-4000-88d5-397db62cea1a" />

</p>

<h3>Step 5: Allow Anyone to Create Tickets</h3>

- Select Settings > User Settings
	- Make sure the following box is unchecked: 
		- Registration Required: Require registration and login to create tickets 
		
<p align="center">
<img width="80%" height="80%" alt="68747470733a2f2f692e696d6775722e636f6d2f6b6364316a52662e706e67 copy" src="https://github.com/user-attachments/assets/fda0222a-a725-469d-ae86-3289f05b06ba" />


<h3>Step 6: Configure Agents</h3>

- Select the Agent tab > Add New Agents
	- Name: Jane Doe
	- Email : jane.doe(@)osticket.com
	- Username: jane.doe
	- Click Set Password and uncheck the box that says "Send the Agent a Password Reset Email"
		- Set your password to anything you like
		- Uncheck the box that says "Require Password Change at Next Login"
		- Select set
		
<p align="center"><img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f665476493052752e706e67 copy" src="https://github.com/user-attachments/assets/6e63ff5e-5d46-4f51-9261-b1889bb66838" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f364f55354b71582e706e67 copy" src="https://github.com/user-attachments/assets/a7086331-65b5-469c-98e5-da900d5c3ed2" />
</p>

- Select the Access tab 
	- Under Primary Department: 
		- Select the Department dropdown menu > System Administrators
		- Select the Role dropdown menu > Supreme Admin
	- Extended Accesss 
		- Select Department > Support > Add > Supreme Admin
- Select Team tab
	- Select Team dropdown menu > Level II Support
	- Select Add
- Select Create	

	
<p align="center">
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f48505350484e552e706e67 copy" src="https://github.com/user-attachments/assets/bab36935-8824-4ab2-af49-7697e7ce2d02" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f686f747831776f2e706e67 copy" src="https://github.com/user-attachments/assets/a3920163-7ae7-45c0-890b-42dd8958994d" />
</p>

- Create another agent and replace Jane with John.
	- Follow the same steps as above, except make some changes to the Primary Department
		- Select the Department dropdown menu > Support
		- Select the Role dropdown menu > View Only
	- Extended Accesss 
		- Select Department > Support > Save Changes
		
<p align="center">
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f715138636b42722e706e67 copy" src="https://github.com/user-attachments/assets/c8a27588-cf26-4d30-b870-34b252e6962d" />
<img width="70%" height="70%" alt="68747470733a2f2f692e696d6775722e636f6d2f4b5650735562342e706e67 copy" src="https://github.com/user-attachments/assets/d7a4b848-e389-41ac-8034-1f375d43c0ad" />
</p>
 
     

<h3>Step 7: Configure Users
</h3>

<p align="center">
<img src="https://i.imgur.com/UUqCK1d.png" height="80%" width="80%" alt="Azure Free Account"/>		
	
- Select the Users tab to create a user
	- Email Address: Karen(@)osticket.com
	- Full Name: Karen Karen
	- Select Add User
	
<p align="center">
<img src="https://i.imgur.com/wpTn12W.png" height="80%" width="80%" alt="Azure Free Account"/>			
	
 - Select the User tab again to create another user
	- Email Address: Ken(@)osticket.com
	- Full Name: Ken Ken
	- Select Add User

<p align="center">
<img src="https://i.imgur.com/EXyy5Gq.png" height="80%" width="80%" alt="Azure Free Account"/>		

<h3>Step 8:  Configure Service Level Agreements (SLA)
</h3>

- We will create three SLAs
- Select the Manage tab > SLA > Add New SLA Plan
	- Name: SEV-A 			
	- Grace Period: 1
	- Schedule dropdown menu: 24/7
	- Select Add Plan
	
<p align="center">
<img src="https://i.imgur.com/fMR4yMR.png" height="80%" width="80%" alt="Azure Free Account"/> <img src="https://i.imgur.com/3tQnihq.png" height="80%" width="80%" alt="Azure Free Services"/>
</p>

	- Name: SEV-B
	- Grace Period: 4
	- Schedule dropdown menu: 24/7
	- Select Add Plan
	
<p align="center">
<img src="https://i.imgur.com/pAbQPEP.png" height="80%" width="80%" alt="Azure Free Account"/>

	- Name: SEV-C 
	- Grace Period: 8
	- Schedule dropdown menu: Monday - Friday 8AM - 5PM with U.S. Holidays
	- Select Add Plan

<p align="center">
<img src="https://i.imgur.com/5cgn0oz.png" height="80%" width="80%" alt="Azure Free Account"/>



<h3>Step 9:   Configure Help Topics
</h3>

- We will create four Help Topics
- Select the Manage tab > Help Topics > Add New Help Topic
	- Business Critical Outage
	- Personal Computer Issues
	- Equipment Request
	- Password Reset
- Select Add Topic for each topic

<p align="center">
<img src="https://i.imgur.com/uFmSyqK.png" height="80%" width="80%" alt="Azure Free Account"/>



✅ Congrats! You have configured osTicket successfully!
