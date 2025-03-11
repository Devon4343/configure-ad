<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

1).Create your resource group for the virtual machine in azure, I choose Windows Server2022 for the domain controller.

2).Remote Desk Top into the virtual machine windows server, virtual machine start menu double click Active Directory Services.

3).Setup a new forest (domain name) then restart the virtual machine, in Active Directory Users and Computers your can create a organizational unit and name the folder _Employees or _Admin.

4).Open PowerShell_ise as an administrator, create a new file and paste the contents of the script, run the script and once finished stop the virtual machine. 

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/2xHOR6A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First created the resource group for the virtual machine, specified my settings to Windows Server2022 with the same network and region. 
</p>
<br />

<p>
<img src="https://i.imgur.com/Ct2LyeM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Log on to the virtual Windows Server, from the start menu go to Active Directory Users and Computers and you can create a new organizational unit for _ADMIN and _EMPLOYEES.
</p>
<br />

<p>
<img src="https://i.imgur.com/sdNi8g3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open PowerShell_ise as an administrator, from a text file you can run a script that will add employees and administration to the Active Directory folder specified.  
</p>
<br />
