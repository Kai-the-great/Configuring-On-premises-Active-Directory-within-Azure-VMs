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
- Launch Domain Controller on Remote Desktop 
- Enable Active Directory on Domain Controller
- Add a new forest as the "domain name"

<h2>Deployment and Configuration Steps</h2>
<img width="1440" alt="Screenshot 2025-01-24 at 2 13 23 PM" src="https://github.com/user-attachments/assets/d8d350c6-161c-4bbf-bb49-d1a789c5ec30" />
</p>
<p>
To create a Windows Server on Microsoft Azure, log in to the Azure portal, click **Create a resource**, and select **Virtual Machine**. Choose the desired Windows Server version, configure the resource group, size, and other settings, then review and deploy the VM. Once deployed, connect to the server using Remote Desktop Protocol (RDP) with the IP address provided in the Azure portal.
</p>
<br />

![image](https://github.com/user-attachments/assets/adeace4c-7a83-465c-98da-7157ed6dd608)


</p>
<p>
While logged into the Domain Controller, Click the >start window and Click >Sever Manager > Then Click >Add roles and Features. Go Through the promts and ensure that the domain controller is selected for "Destination Sever". Under Sever Roles select; "Active Directory Domain Services", finish going through the prompts by clicking next and restart the Virtual Machine.  
</p>
<br />
<img width="1440" alt="Screenshot 2025-01-17 at 3 13 51 PM" src="https://github.com/user-attachments/assets/eb7aa4bc-1df8-4758-9d04-b6a8ef1f5526" />

</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
