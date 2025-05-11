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
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Reload IIS than Enable: php_imap.dll, php_intl.dll, php_opcache.dll.After this you will need to Rename: ost-config.php:
  
- From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
- To: C:\inetpub\wwwroot\osTicket\include\ost-config.php

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, install HeidiSQL:
  
- Open Heidi SQL
- Create a new session, root/root
- Connect to the session
- Create a database called “osTicket”

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Continue Setting up osTicket in the browser:
  
- MySQL Database: osTicket
- MySQL Username: root
- MySQL Password: root
- Click “Install Now!”

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
osTicket is now installed! Browse to help desk login page: http://localhost/osTicket/scp/login.php

</p>
<br />
