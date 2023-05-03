<p align="center">
 <img src="https://i.imgur.com/7qSYnb1.jpg" height="80%" width="80%" alt="VM logo"/>
</p>

<h1>Creating a Virtual Switch</h1>


<h2>Description</h2>
In our previous demonstration, we dabbled in the world of virtual machines. Today, we're going to take it up a notch and create not just one, but two virtual switches!

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
From Server Manager, select Tools > Hyper-V Manager.
 <br/>
<img src="https://i.imgur.com/B7SxtGm.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Underneath Hyper-V manager, highlight and right-click your Hyper-V host server, in this demonstration it's CORPSERVER and select Virtual Switch Manager.
 <br/>
<img src="https://i.imgur.com/cwHMgol.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
With New virtual network switch highlighted, select Private.
Select Create Virtual Switch.

 <br/>
<img src="https://i.imgur.com/ajPjZaz.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
In the Name field, use Switch 1 or name it whatever you'd like and select Apply.

<br/>
<img src="https://i.imgur.com/J0bG2OG.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
You can also reach the Virtual Machine manager under the actions pane. See picture below.
 <br/>
<img src="https://i.imgur.com/KbEAtDa.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
This next virtual switch is going to be external. Highlight it and click "create virtual switch"

 <br/>
<img src="https://i.imgur.com/6waqImd.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
Name your virtual switch and press okay. Great, we are finished! Good job!
 <br/>
<img src="https://i.imgur.com/gjcMXTu.png" height="80%" width="80%" alt="DHCP"/>
<br />
<br />
I hope you enjoyed this demonstration.
 <br/>
<img src="https://i.imgur.com/pS8SYQI.jpg" height="80%" width="80%" alt="DHCP"/>
<br />
<br />

 
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
