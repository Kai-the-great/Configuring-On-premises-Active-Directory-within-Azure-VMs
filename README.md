<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1> Active Directory Deployed (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create a Domain Controller on Microsoft Azure
-  Enable Active Directory on Domain Controller
- Add a new forest as the "domain name"
- Restart Virtual Machime using "Domain Name\UserName"

<h2>Deployment and Configuration Steps</h2>
<img width="1440" alt="Screenshot 2025-01-24 at 2 13 23 PM" src="https://github.com/user-attachments/assets/d8d350c6-161c-4bbf-bb49-d1a789c5ec30" /> <img width="1440" alt="Screenshot 2025-01-28 at 12 53 26 PM" src="https://github.com/user-attachments/assets/fd65df49-fd2c-4693-9348-f5b297025bc2" />

</p>
<p>
To create a Windows Server on Microsoft Azure, log in to the Azure portal, click Create a resource, and select Virtual Machine. Choose the desired Windows Server version, configure the resource group, size, and other settings, then review and deploy the VM. Once deployed, connect to the server using Remote Desktop Protocol (RDP) or Microsoft Remote Desktop (for Mac) with the IP address provided in the Azure portal.
</p>
<br />

</p>


<img width="1440" alt="Screenshot 2025-01-28 at 12 38 57 PM" src="https://github.com/user-attachments/assets/f9752035-5d9c-4a0d-99b5-f4eef179d6ba" />





</p>
<p>
While logged into the Domain Controller, click Start, then open Server Manager. Click Add Roles and Features and proceed through the setup prompts, ensuring the Domain Controller is selected as the Destination Server. Under Server Roles, select Active Directory Domain Services (AD DS), complete the remaining prompts, and restart the Virtual Machine when prompted. 
</p>
<br 

  <![DEBF6B2B-2556-4D2D-90A2-92A12D1CF2A1_1_201_a](https://github.com/user-attachments/assets/512f4870-b0e0-4fb1-a128-092665045b4a)

</p>
<p>
After restarting, a notification flag will appear, prompting you to complete the configuration wizard. Click Promote this server to a domain controller, then select Add a new forest and enter the desired domain name. Click Next and follow the setup steps to finalize the configuration.
</p>

<img width="1440" alt="Screenshot 2025-01-28 at 1 30 32 PM" src="https://github.com/user-attachments/assets/3288f86f-de4d-45cf-9359-e24c427b1596" />
<p>
Once all configurations are complete, restart the Domain Controller. Log in using the domain name and the administrator credentials set during the new forest setup.
</p>


<br />
