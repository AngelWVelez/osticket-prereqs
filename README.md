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

- Create an Azure Virtual Machine Windows 10, 4 vCPUs
- Log into the VM with Remote Desktop
- Have osTicket-Installation-Files
- Install / Enable IIS in Windows WITH CGI

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/hnalqjC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder:
  
- install PHP Manager for IIS 

</p>
<br />

<p>
<img src="https://i.imgur.com/Y8U3HuO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder:

-  install the Rewrite Module (rewrite_amd64_en-US.msi)

</p>
<br />

<p>
<img src="https://i.imgur.com/Gx8TUp1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the C drive:
  
- Create the directory C:\PHP

</p>
<br />

<p>
<img src="https://i.imgur.com/p46gTHt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder:
  
- unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder

</p>
<br />

<p>
<img src="https://i.imgur.com/p1gzsHn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  
From the “osTicket-Installation-Files” folder:

-   install VC_redist.x86.exe.

</p>
<br />

<p>
<img src="https://i.imgur.com/T5zhXPz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder:
  
- install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
- Typical Setup
- Launch Configuration Wizard (after install)
- Standard Configuration

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is now installed! Browse to help desk login page: http://localhost/osTicket/scp/login.php

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is now installed! Browse to help desk login page: http://localhost/osTicket/scp/login.php

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is now installed! Browse to help desk login page: http://localhost/osTicket/scp/login.php

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is now installed! Browse to help desk login page: http://localhost/osTicket/scp/login.php

</p>
<br />
