# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- osTicket Installation files
- Heidi SQL

<h2>Installation Steps</h2>

<p>Ok, welcome to my first tutorial! First things first we will have to create a Virtual machine using the Microsoft Azure portal. We will be using a VM which is a remote computer. We are using a VM in order to protect our physical machine just in case something breaks. Create a resource group and title it "osTicket". Afterwards create a VM with 2-4 CPUs. In this example I will be using 4 CPUs.
<img src= "https://i.imgur.com/0cr8OEx.jpg="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>Next simply connect to your newly created VM using RDP using the public IPv4 address. If you are a Mac user you will have to download Microsoft RDP.
<br
<p>
<img src="https://i.imgur.com/uLVKzxS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Alright, now that you are connected to your VM you will have to enable IIS. Simply access the control panel then select uninstall a program. Off to the left select "Turn windows features on or off". A list will appear then you will enable Internet Information Services.
</p>
<br />

<p>
<img src="https://i.imgur.com/qtEnuWu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 
 Excellent. Now that you have enabled IIS we need to install Web Platform Installer                                                                                               
<img src="https://i.imgur.com/AxHCfQ6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
                                                                                                 
Once you have installed Web Installer Platform open it. From inside the application you are going to install MySQL 5.5 Afterwards install x86 version of PHP up until 7.3. There are some failed files such as C++ redistributable package as well as PHP 7.3.8 and PHP Manager for IIS those files can be found with the install link.
                                                                                                 
<img src="https://i.imgur.com/JJ8bZeJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
                                                                                                 

 Next download osTicket. Then extract and copy the "upload" folder into c:\inetpub\wwwroot. Afterwards rename the folder to osTicket
                                                           
<img src="https://i.imgur.com/TUGiSKi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>                                                          
                                                                                                 

                                                                                                 
Open IIS Manager and restart the server. Once inside IIS manager go to Sites->Default->osTicket on the right, click "Browse*.80" from there your default browser should open osTicket webserver.                                                                                                
       
                                                                                                                                
<img src="https://i.imgur.com/4AkTkV0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />                                                                                                                                
                                                                                                                                                       
