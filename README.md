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

- Azure Subscription/ Azure Free trial
- <a href="https://github.com/RonaldCarter/PHPManager/releases/tag/V1.5.0">PHP Manager</a>
- <a href="https://www.iis.net/downloads/microsoft/url-rewrite">Rewrite Module</a>
- <a href="https://windows.php.net/download#php-8.1">PHP Distribution Package</a>
- <a href="https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170#latest-microsoft-visual-c-redistributable-version">Visual C++ Redistributable</a>
- <a href="https://downloads.mysql.com/archives/community/">MySQL</a>
- <a href="https://osticket.com/download/">osTicket</a>
- <a href="https://www.heidisql.com/download.php">HeidiSQL</a>

<h2>Installation Steps</h2>
<p>Step 1:</p>
<p>
Navigate the Azure Portal to create a Windows 10 Virtual Machine. To tailor your specific requirements, you can configure a virtual machine with your preferred settings, including image size, memory, vCPU count, OS disk type, and more. Be sure to write down your virtual machine's username and password for future access.
</p>
<p>
<img src="https://i.imgur.com/11la5cH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>Step 2:
<p>To find your virtual machine's IP address, open Virtual Machines in the Azure portal, select the desired VM, and go to the Overview tab. Write down the Public IP address displayed there.

Then, open Remote Desktop Protocol (RDP) on your computer, enter the IP address, and use the username and password you saved earlier to log in to your virtual machine.
<p>
<img src="https://i.imgur.com/hwhcJAr.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>Step 3:</p>
<p>
Start by opening the Control Panel, then click on Programs, followed by Programs and Features. Click on Turn Windows features on or off, check the box next to Internet Information Services (IIS), then expand World Wide Web Services > Application Development Features, and check the box next to CGI. Finally, click OK to enable IIS and CGI.
<p/>
<p>
<img src="https://i.imgur.com/ybAhzcJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>Step 4:</p>
<p>Download the PHP Manager application from the provided list of prerequisites and follow the installation instructions to set it up on your system, ensuring all necessary configurations are completed for proper functionality.</p>
<img src="https://i.imgur.com/0WHDEVT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 5:</p>
<p>Download the rewrite module from the provided list of requisites, making sure to select the 64-bit version that corresponds to the language of your preference, and follow the installation instructions to set it up on your system, ensuring all necessary configurations are completed for proper functionality.</p>
<img src="https://i.imgur.com/Avgmr7E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 6:</p>
<p>Navigate to the C drive by opening File Explorer and selecting This PC or Computer. Once you are in the C drive, right-click in an empty space and choose New > Folder. Name the new folder PHP and press Enter to create the directory.</p>
<img src="https://i.imgur.com/7QUVVp3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>It should end up looking like the image below.</p>
<img src="https://i.imgur.com/ITojMXZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 7:</p>
<p>Download the 8.1.30 x64 PHP distribution package from the official PHP website for Windows. </p>
<img src="https://i.imgur.com/TTr7NHg.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 8:</p>
<p>Right-click on the PHP distribution package, select Extract All..., and choose the PHP directory on your C drive as the destination for the extracted files.</p>
<img src="https://i.imgur.com/S5Mzq6F.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 9:</p>
<p>Download the latest supported Microsoft Visual C++ Redistributable from the provided list of prerequisites, then follow the installation instructions to set it up on your system, ensuring that all necessary configurations are completed for proper functionality."</p>
<img src="https://i.imgur.com/AD3mXD1.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 10:</p>
<p>Download the latest MySQL from the provided list of requisites, and follow the installation instructions making sure to select a typical setup.</p>
<img src="https://i.imgur.com/KT0rBr8.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 11:</p>
<p>Open the MySQL application and select Standard Configuration. Next, choose Install as a Windows Service and select Modify Security Settings to create a root password. Be sure to write down your root password. Finally, click Execute to start the setup and Finish to complete the configuration process.</p>
<img src="https://i.imgur.com/D3wnvYm.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/BBTb6SD.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xFeQDgn.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 13:</p>
<p>Open IIS as an administrator.</p>
<img src="https://i.imgur.com/u0duRYQ.png" height = "80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 14:</p>
<p>Click the PHP Manager and then register a new PHP version and select the php-cgi.exe in the PHP folder.</p>
<img src="https://i.imgur.com/MxlOkoJ.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/xAyytUQ.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/zm1btvf.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 15:</p>
<p>Reload the IIS by pressing stop then start</p>
<img src="https://i.imgur.com/Lyxy5IF.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>


<p>Step 16:</p>
<p>Click on the </p>
<img src="https://i.imgur.com/8OEk1yE.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/nsuZtao.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 17:</p>
<p>Next we will extract the osTicket Installation files we just downloaded</p>
<img src="https://i.imgur.com/zGkNkEE.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>
<p>You should be left with two files like the image below</p>
<img src="https://i.imgur.com/JpeU3pp.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 18:</p>
<p>Within the osTicket Installation files we will copy the upload folder and paste it into c:\inetpub\wwwroot</p>
<p>It should look like the image below.</p>
<img src="https://i.imgur.com/0d2TWcm.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>


<p>Step 19:</p>
<p> Right-click the upload file we just copied and pasted. And rename the upload file to "osTicket"</p>
<img src="https://i.imgur.com/AlikC1Z.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>
<p>It should look like the image below</p>
<img src="https://i.imgur.com/6As8Oef.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 20:</p>
<p>Open the IIS manager as an admin and reload the IIS by pressing stop and then start</p>
<img src="https://i.imgur.com/Lyxy5IF.png" height = "90%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 21:</p>
<p>Make sure on the left-hand side you expand the osTicket-vm, then expand the sites folder, then expand the Default Web Site. Finally, click on the osTicket Folder</p>
<img src="https://i.imgur.com/BF6RjGn.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>Next click on the "Browse*.80(http)"</p>
<img src="https://i.imgur.com/d3pPrQp.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>You should get to a website that looks like the image below</p>
<img src="https://i.imgur.com/l7uAhhV.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>

<p>Step 22:</p>
<p>Go back to the IIS. Make sure you are still on osTicket folder and click PHP Manager</p>
<img src="https://i.imgur.com/BexTjJ3.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>Next click on the enable or disable and extension</p>
<img src="https://i.imgur.com/Tz41mmi.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>Right-click and enable the following extensions:</p>
<p>- php_imap.dll</p>
<p>- php_intl.dll</p>
<p>- php_opcache.dll</p>
<img src="https://i.imgur.com/8NH5pyx.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>Refresh the osTicket web browser to see the changes. If not try to reload the IIS manager.</p>

<p>Step 23:</p>
<p>First, open File Explorer on your computer. In the address bar at the top, type C:\inetpub and press Enter. Once there, open the wwwroot folder, then navigate to the osTicket folder inside it. Finally, open the include folder. Now you’re in C:\inetpub\wwwroot\osTicket\include.</p>
<p>Once in the include folder, right click the "ost-sampleconfig.php" and rename it to "ost-config.php. When done it should look like the example below</p>
<img src="https://i.imgur.com/CNd129C.png" height = "70%" width="70%" alt="Disk Sanitization Steps"/>
<p>Right-click a file and click Properties. You will see details about the file, including its size, type, location, date created, and date modified. Click the Security tab and click Advanced. </p>
<img src="https://i.imgur.com/xU3ZbvZ.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>This will open the Advanced Security Settings window, where you can adjust detailed permissions, view the file's ownership, and manage special permissions and auditing settings. Click Disable inheritance in the Advanced Security Settings window. This option will let you manage permissions independently by stopping the file or folder from automatically inheriting permissions from its parent folder. After clicking Disable inheritance, select Remove all inherited permissions from this object.</p>
<img src="https://i.imgur.com/7zfVs4c.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Next, click Add to create a new permission entry.</p>
<img src="https://i.imgur.com/CpMxOb4.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p> In the Permission Entry window, click Select a principal to choose a user or group to assign permissions.</p>
<img src="https://i.imgur.com/lt0HWlH.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>For the sake of this lab we will enter the object name as everyone. However, this is not recommended in real-life business practice. Afte clicking check names, click ok.</p>
<img src="https://i.imgur.com/dK6NHQo.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Next check the full control box and click ok.</p>
<img src="https://i.imgur.com/F6IVIaX.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Click apply and ok</p>
<img src="https://i.imgur.com/PCbm0GR.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Click Ok</p>
<img src="https://i.imgur.com/b51Mva2.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>

<p>Step 24:</p>
<p>Download HeidiSQL from the list of prerequisites and follow all the steps to complete the installation.</p>
<img src="https://i.imgur.com/qqj86ml.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Once the application is installed, it should look like the application below.</p>
<img src="https://i.imgur.com/5P887Rt.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>

<p>Step 25:</p>
<p>Once you're in HeidiSQL, click "New" to create a session.</p>
<img src="https://i.imgur.com/I51JBsw.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>You will find yourself in a screen like the image below. Next, input the password from the MySQL server we made in step 12. Lastly, press open to connect to the session.</p>
<img src="https://i.imgur.com/cu3n20J.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>

<p>Step 26:</p>
<p>Once you are connected to the session. Right-click the session which is called Unnamed, press 'create new', and then press "database".</p>
<img src="https://i.imgur.com/3rMTbKH.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Name the new Database "osTicket", and press ok.</p>
<img src="https://i.imgur.com/Ftm9pk1.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>

<p>Step 27:</p>
<p>Go back or reopen the osTicket installer and click continue.</p>
<img src="https://i.imgur.com/iWtHv8u.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>
<p>Configure osTicket to your liking, however, make sure that the MySQL Database name is osTicket, and the MySQL username and password are the once you configured for the MySQL database in step 12.</p>
<img src="https://i.imgur.com/Qzp40K6.png" height = "50%" width="50%" alt="Disk Sanitization Steps"/>

<p>Congrats, You have installed osTicket. You can now create a ticket using http://localhost/osTicket/. Or login into the agent portal using http://localhost/osTicket/scp/login.php.</p>












<br />
