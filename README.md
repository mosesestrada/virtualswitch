<p align="center">
 <img src="https://i.imgur.com/WsQoR9W.jpg" height="80%" width="80%" alt="VM logo"/>
</p>

<h1>Creating a DHCP relay</h1>


<h2>Description</h2>
In our previous demonstration, we dabbled in the world of virtual machines. Today, we're going to take it up a notch and create not just one, two virtual switches!

Think of a virtual switch as the glue that binds virtual machines together. It functions just like its physical counterpart, except it links virtual machines instead of physical devices.

Now, there are three types of virtual switches that you need to know. The first is the private virtual switch which allows virtual machines to communicate with each other exclusively. Then there's the internal virtual switch that connects virtual machines with the host. Lastly, there's the external virtual switch, which connects everything from the host to the virtual machines, and even the internet!

For today's lesson, we're going to focus on creating two of these bad boys. We'll set up a private virtual switch and an external virtual switch, and trust me when I say it's going to be a breeze. Get ready to dive into the exciting world of virtual switches!
<br />

<h2>Environments Used </h2>

 <b>Windows Server 2019 </b> <p>
 <b>Hyper-V</b></p>

<h2>Program walk-through:</h2>

<p align="center">


<br />
From Server Manager, select Tools > Routing and Remote Access.
Expand IPv4.
 <br/>
<img src="https://i.imgur.com/S2CseAY.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Expand IPv4. Right-click General and select New Routing Protocol.
 <br/>
<img src="https://i.imgur.com/sMHK1Or.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Select DHCP Relay Agent and then select OK.

 <br/>
<img src="https://i.imgur.com/KVEBXfg.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
From the left pane, right-click DHCP Relay Agent and select New Interface.
Select NetTeam and then select OK.

<br/>
<img src="https://i.imgur.com/JlEw6TU.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Make sure Relay DHCP packets is selected.
Set the boot threshold to 0 (zero).
Select OK.

 <br/>
<img src="https://i.imgur.com/lPYyMCk.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Right-click DHCP Relay Agent and select Properties.

 <br/>
<img src="https://i.imgur.com/GynvPMW.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
In the Server address field, enter the IP address of the DHCP server. The IP address of the DHCP server I am targeting is 192.168.0.14.
Select Add and then select OK.
 <br/>
<img src="https://i.imgur.com/GEFKCol.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Lastly we verify we're getting an IP address from the DHCP server. I do a quick /ipconfig at the powershell prompt and get an APIPA address. No worries, all I have to do is follow up with a /ipconfig /release & an ipconfig /renew and VIOLA I get a functional IP address.
 <br/>
<img src="https://i.imgur.com/kLulX91.png" height="80%" width="80%" alt="DHCP"/>

<br />
<br />
Hope you enjoyed this demonstration.
 <br/>
<img src="https://i.imgur.com/dJzDtPN.jpg" height="80%" width="80%" alt="DHCP"/>

 
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
