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
<img src="https://i.imgur.com/SChp8Go.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open IIS as an Admin:

- Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)

</p>
<br />

<p>
<img src="https://i.imgur.com/jFTfOfB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server)

</p>
<br />

<p>
<img src="https://i.imgur.com/wb8B9C2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install osTicket v1.15.8:
  
- From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip”
- copy the “upload” folder into “c:\inetpub\wwwroot”
- Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”

</p>
<br />

<p>
<img src="https://i.imgur.com/MXrKrSI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS (Open IIS, Stop and Start the server)

- Go to sites -> Default -> osTicket
- On the right, click “Browse *:80”

</p>
<br />
<p>
<img src="https://i.imgur.com/hVBs6vD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Note that some extensions are not enabled

</p>
<br />
<p>
<img src="https://i.imgur.com/ALG8n4S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable extensions:
  
- Go back to IIS, sites -> Default -> osTicket
- Double-click PHP Manager
- Click “Enable or disable an extension”
- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll
- Refresh the osTicket site in your browser, observe the changes

</p>
<br />

<p>
<img src="https://i.imgur.com/rlS6KgK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename: ost-config.php:
  
- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

</p>
<br />

<p>
<img src="https://i.imgur.com/UxrrAr8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Assign Permissions: ost-config.php:
  
- Disable inheritance -> Remove All

</p>
<br />

<p>
<img src="https://i.imgur.com/srjIpK4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Assign Permissions: ost-config.php:
  
- New Permissions -> Everyone -> All

</p>
<br />

<p>
<img src="https://i.imgur.com/diyFO4U.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue Setting up osTicket in the browser (click Continue):
  
 - Name Helpdesk
 - Default email (receives email from customers)

</p>
<br />

<p>
<img src="https://i.imgur.com/I8WEQcj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder:
  
- Install HeidiSQL.
- Open Heidi SQL
- Create a new session, root/root
- Connect to the session
- Create a database called “osTicket”

</p>
<br />
<p>
<img src="https://i.imgur.com/cn0ZaHz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue Setting up osTicket in the browser:
  
- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: root
- Click “Install Now!”

</p>
<br />

</p>
<br />
<p>
<img src="https://i.imgur.com/1m00kCE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
OsTicket is now installed!
