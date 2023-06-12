<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create two VM's. One with Windows and one with Linux.
- Remote connect to the Windows' VM and download Wireshark.
- Input different commands to see how the interactions between two networks work.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/r1QtqzR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create two VM's. one with Windows and one with Linux.
</p>
<br />

<p>
<img src="https://i.imgur.com/VaSlW00.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to "virtual machines" on azure> go to the Windows' VM> copy the public IP address> Open "Remote Desktop Connection"> Paste the Copied IP address onto "RDC"> log in with credentials created when VM was created.
</p>
<br />

<p>
<img src="https://i.imgur.com/r1fVHkR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Once logged in, download Wireshark onto VM.
</p>
<br />

<p>
<img src="https://i.imgur.com/P7AMBG8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open WireShark> Press Blue shark icon on the top left> Watch traffic unfold. After, type "icmp"(make sure is all lower case, otherwise it won't work).
</p>
<br />

<p>
<img src="https://i.imgur.com/bULBIFl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
It should not show any traffic because ICMP is the protocol ping uses. So the only way to see traffic through ICMP is to ping a network.
</p>
<br />

<p>
<img src="https://i.imgur.com/VXqblGE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p> 
  On host PC go to azure>linux-VM>copy PRIVATE ip. Then go back into the open VM> Windows search bar> Type "command prompt"> then inside of the command prompt, type "ping (paste the copied private IP address)
</p>
<br />

<p>
<img src="https://i.imgur.com/fPBsGjY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to wireshark and Watch the traffic because now the "icmp" protocol is being used through ping.
</p>
<br />

<p>
<img src="https://i.imgur.com/hNp5vza.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
cdvfsdfgdfzgdszgfdzgggggggggggggggggggggggggggggggggggggggggggggggggfdzgfdzgdzfgdfzgdzfgrdzfgzzzz
</p>
<br />

<p>
<img src="https://i.imgur.com/anBekKI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to host PC> Azure> Type on Azure's search bar "Network Security Groups" Click on linux VM's group>Click "inbound security rules"> Then click "add"
</p>
<br />

<p>
<img src="https://i.imgur.com/uCzkh9D.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/WBDRAfv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://i.imgur.com/RlYC2Kq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
