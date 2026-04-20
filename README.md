<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket. The project demonstrates the osTticket help desk system in a cloud-hosted enviornment by using Microsoft Azure.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 11 for Desktop
- Windows 10 for Virtual Machine</b> (22H2)

<h2>List of Prerequisites</h2>

- Azure Subscription
- Azure Virtual Machine
    - OS: Windows 10
    - vCPUs: 4
- Remote Desktop Connection
  
<h2>Installation Steps</h2>

### Step 1: Create and Configure the Azure Virtual Machine
<p>

<img width="1837" height="846" alt="image" src="https://github.com/user-attachments/assets/d4526df4-3ff5-48fc-b2f1-aa3bc52d23d3" />

</p>
<p>
Logged into Azure to start creating my enviornment for osTicket. Created a Resource Group called "osTicket" for where the Virtual Machine and Virtual Network will be located.
</p>
<br />

<p>

<img width="1873" height="924" alt="image" src="https://github.com/user-attachments/assets/6e13ea6d-bf7f-48e1-82af-092d9ad8f3d9" />

</p>
<p>
After creating the resource group I needed to create a virtual network for my setup on the Virtual Machine. I called the network "ticket-vnet" and put it into the resource group.
</p>
<br />

<p>
<img width="1874" height="881" alt="image" src="https://github.com/user-attachments/assets/8de4c4a8-9a73-4284-bac0-17cbccdc6670" />
</p>
<p>
Creating the a Virtual Machine called "ost-vm". Using the resource group made before (osTicket) and put it there. I'm also using "West US 2" as my region because that is closest to me for quicker feedback, but can be done in a different Region. 
</p>
<br />

<p>
<img width="1865" height="877" alt="image" src="https://github.com/user-attachments/assets/26c6243c-1634-43bc-95da-ca60f81f1312" />
</p>
<p>
For the Image/OS I used Windows 10 Enterprise, version 22H2 - x64 Gen2. For Size I used Standard_L4aos_v4 - 4 vcpus, 32 GiB memory (Note: I have done it before on 2vcpus and 16 GiB memory, but its slower and cheaper).
    
> [!NOTE]
> I have done it before on 2vcpus and 16 GiB memory, but its slower and cheaper.
</p>
<br />

<p>
<img width="1870" height="879" alt="image" src="https://github.com/user-attachments/assets/0da4fb5a-2c73-48d3-9af2-9259f71dd623" />
</p>
<p>
For logging into the Virtual Machine you need a Username and Password. 
    - Username: labuser
    - Password: Cyberlab123!

Since I'm using a Windows 10/11 OS I need to check the licensing at the bottom. The usernames and passwords I use are for this project only. Its never good to store your passwords in plain text.
</p>
<br />




