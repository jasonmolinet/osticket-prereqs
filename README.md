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

- Windows 10 Pro

<h2>Installation Steps</h2>

Step 1:


![image](https://i.imgur.com/wAPhqS1.jpg)


Create Virtual Machine in Azure
- Create a new resource group 
- Create a Windows 10 Pro virtual machine (VM) with 4 virtual CPUs as the size
- Remember and take note of the username and password created
- Under the network tab, allow it to create a new virtual network (vnet)
- Then hit review and create!

Step 2:


![image](https://i.imgur.com/czGO2h6.jpg)


Installation
- Connect to the VM via remote desktop connection application
- Login with saved username and password
- While in the VM, open microsoft edge and open this link that includes the installation files for osTicket: https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
- Now open control panel > programs > programs and features > turn windows features on or off > then check internet information services then expand to world wide web services then application development features then check "CGI" then under "common http features" under world wide web services make sure everything is checked
- To make sure it works, go to the edge browser to 127.0.0.1 in the url then it will load the windows Internet Information Services (IIS) page

Step 3:


![image](https://i.imgur.com/LhCoLYc.jpg)


osTicket Installation Files
- Go to installation files for osTicket: https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6
- Download "PHPManagerforIIS" then install to VM
- Download "rewrite" then install to VM
- Then go to files under the C: folder create a new folder called PHP
- Download PHP.zip and unzip in the created folder called PHP
- Download VC_redist and install
- Download MySQL and install


Step 4:


![image](https://i.imgur.com/CAmCq5p.jpg)


MySQL and PHP Manager
- Launch SQL and choice standard config
- Write down username: root and password: Password1
- Hit execute then finish
- Launch IIS as admin then open PHP Manager
- Register new PHP version and find the C: in the PHP folder in the new window
- Click php-cgi
- Reminder to hit restart on the top right to refresh server


Step 5:

osTicket and PHP Manager
- 
