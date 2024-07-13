<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>List of Prerequisites</h2>

- Enable IIS (Internet Information Services)
- Install Web Platform Installer
- Install MySQL 5.5.62
- Configure permissions and Install OS Ticket

<h2>Installation Steps</h2>

<p>
<a href='https://postimg.cc/XBfv8F7r' target='_blank'><img src='https://i.postimg.cc/XBfv8F7r/Screen-Shot-2024-07-06-at-1-11-38-PM.png' height="80%" width="80%" border='0' alt='Screen-Shot-2024-07-06-at-1-11-38-PM'/></a>  
</p>
<p>
Main steps is to create a resource group where you can store, manage and organize resources like virtual machines, databases, and storage accounts in a unified manner. Create a Windows 10 Virtual Machine (VM) with 2-4 Virtual CPUs. Make sure to select a plan that is suffient but also beware of monthly cost. When creating the VM, it is important to allow the Azure cloud platform to create a new Virtual Network (Vnet) before moving forward to creating the second VM so you can use the same (VNet) with both machines . 

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the next step with be to create a remote desktop conection where we will install the necessary software inside of the VM. If you are using a Mac, you will have to download Mircrosoft remote desktop. In this section we will be dowloading IIS (Internet information services), PHP manager for IIS, Rewrite module, PHP-7.3.8, VC_redist.x86.exe, and MySQL 5.5.62 . All of the download instructions are provided separately, because it is too much to list. These installs will be necessary to instal the actaul OsTicket platform in the next step.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, I will be downloading the OS Ticket software and following the upload instructions. All necessary software needed to run Osticket has been installed and configured.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
