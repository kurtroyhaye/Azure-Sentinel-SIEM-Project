<h1>Azure Sentinel (SIEM) </h1>

<h2>Description</h2>
In this project I setup Azure Sentinel (SIEM) and connect it to a live virtual machine named honey pot. Here we will observe live attacks (RDP Brute Force) from all around the world. We will also use a custom PowerShell script to look up the attackers Geolocation information and plot it on the Azure Sentinel Map!
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Mircrosoft Azure</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Microsoft Azure Virtual Machine Setup: <br/>
<img src="https://i.imgur.com/1CrMhGt.jpg" height="80%" width="80%" alt="Virutal Machine Setup Steps"/>
<br />
<br />
Creating Log Analytics Worspace:  <br/>
<img src="https://i.imgur.com/oM1p1Yb.png" height="80%" width="80%" alt="Log Analytics Worspace"/>
<img src="https://i.imgur.com/ZWitC0A.png" height="80%" width="80%" alt="Log Analytics Worspace"/>
<br />
<br />
Workspace Configuration: <br/>
<img src="https://i.imgur.com/hafm2p5.png" height="80%" width="80%" alt="Workspace Configuration"/>
<img src="https://i.imgur.com/vQSkWmW.png" height="80%" width="80%" alt="Workspace Configuration"/>
<br />
<br />
Connecting to Virtual Machine:
 <br/>Firewall was disable to allow VM to be susceptible to attack<br/><br/>
<img src="https://i.imgur.com/jShPXPr.png" height="80%" width="80%" alt="Virtual Machine"/>
<img src="https://i.imgur.com/JUyDnNM.png" height="80%" width="80%" alt="Virtual Machine"/>
<img src="https://i.imgur.com/otP8Nsa.png" height="80%" width="80%" alt="Virtual Machine"/>
<br />
<br />
View logs in Event Viewer:  <br/>
<img src="https://i.imgur.com/lg26CqK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Login to ipgeolocation.io:  <br/>
<img src="https://i.imgur.com/DRJGL3X.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Execute Custom Security Log Exporter in Powershell: <br/><br/>
[https://github.com/kurtroyhaye/Custom-Security-Log-Exporter]
<br/>
<img src="https://i.imgur.com/IPMJnAR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Custom Log (Import Event Log into Log Analytics Workspace):  <br/>
<img src="https://i.imgur.com/N3Qbd7J.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run custom log in log analytics workspace:  <br/>
<img src="https://i.imgur.com/sVzyvuJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Extract Raw Data in log analytics workspace:  <br/>
<img src="https://i.imgur.com/Sa6U9tZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Geo Map workbook in Azure Sentinel:  <br/>
<img src="https://i.imgur.com/ANKwZRQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 
<br/>

</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
