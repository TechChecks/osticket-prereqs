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
<a href='https://postimg.cc/30YFgcWD' target='_blank'><img src='https://i.postimg.cc/30YFgcWD/Files-installed-2024-07-12-at-9-11-58-PM.png' height="80%" width="80%" border='0' alt='Files-installed-2024-07-12-at-9-11-58-PM'/></a></p>
<p>
In the next step with be to create a remote desktop conection where we will install the necessary software inside of the VM. If you are using a Mac, you will have to download Mircrosoft remote desktop. In this section we will be dowloading IIS (Internet information services), PHP manager for IIS, Rewrite module, PHP-7.3.8, VC_redist.x86.exe, and MySQL 5.5.62 . All of the download instructions are provided separately, because it is too much to list. These installs will be necessary to install the actaul OsTicket platform in the next step.
</p>
<br />

<p>
<a href='https://postimg.cc/RNXNdVg0' target='_blank'><img src='https://i.postimg.cc/RNXNdVg0/os-ticket-installer-2024-07-12-at-10-11-06-PM.png' height="80%" width="80%" border='0' alt='os-ticket-installer-2024-07-12-at-10-11-06-PM'/></a></p>
<p>
In this step, I will be downloading the OS Ticket software and following the upload instructions. All necessary software needed to run Osticket has been installed and configured.
</p>
<br />

<p>
<a href='https://postimg.cc/8JYvmz5r' target='_blank'><img src='https://i.postimg.cc/8JYvmz5r/Screen-Shot-2024-07-12-at-11-01-45-PM.png' height="80%" width="80%" border='0' alt='Screen-Shot-2024-07-12-at-11-01-45-PM'/></a></p>
<p>
OsTicket has successfully been installed. In the following steps, I will be assigning privelidges to different agents and users for tickets that will need to be resolved. 
</p>
<br />

<p>
<a href='https://postimg.cc/rKWf1r8S' target='_blank'><img src='https://i.postimg.cc/rKWf1r8S/Untitled-design-5.png' height="80%" width="80%" border='0' alt='Untitled-design-5'/></a>
<p>
Here we are configuring roles for Admins/agents and users. Admin roles would be able to create, delete, edit and close tickets etc.. Obiviously for higher ranked personel such as admins, there would be more permissions granted than agents without. Here you can see the set up for Admins, agents and users.
</p>
<br />

<p>
<a href='https://postimg.cc/Dmp5s3t3' target='_blank'><img src='https://i.postimg.cc/Dmp5s3t3/SLAand-Helpdesktopics.png' height="80%" width="80%" border='0' alt='SLAand-Helpdesktopics'/></a>
<p>
A very important part of the ticketing process is the SLA (Service Level Agreement). SLA's can be for anything. For instance, part of your SLA can set a minimum resolution time for tickets. We will also create different severity levels. In this section, I also added different help topics that the end users may need help with from support. 
</p>
<br />

<p>
<a href='https://postimg.cc/WhKzLLns' target='_blank'><img src='https://i.postimg.cc/WhKzLLns/End-User.png' height="80%" width="80%" border='0' alt='End-User'/></a>
<p> 
Here us an example of the OsTicketing system where the end user has submitted a help desk ticket from the end users URL. We would then receive the ticket at the help desk and proceed to resolve the issue at hand within the scope or our abilities.

