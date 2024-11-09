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
- <a href="https://windows.php.net/downloads/releases/">PHP Distribution Package</a>
- Item 5

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
<img src="https://i.imgur.com/ITojMXZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 7:</p>
<p>Navigate to the C drive by opening File Explorer and selecting This PC or Computer. Once you are in the C drive, right-click in an empty space and choose New > Folder. Name the new folder PHP and press Enter to create the directory.</p>
<img src="https://i.imgur.com/7QUVVp3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p>Step 8:</p>
<p>Download the PHP Distribution Package from the provided list of requisites</p>
<img src="https://i.imgur.com/bi0xVeV.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>

<p>Step 9:</p>
<p>Right-click on the PHP distribution package, select Extract All..., and choose the PHP directory on your C drive as the destination for the extracted files.</p>
<img src="https://i.imgur.com/S5Mzq6F.png" height = "60%" width="60%" alt="Disk Sanitization Steps"/>






<br />
