<h1>Installing a RADIUS Server</h1>


<h2>Description</h2>
In this lab, I learned to install a RADIUS server. RADIUS (Remote Authentication Dial-In User Service) was initially designed to provide full AAA (authentication, authorization, and accounting) support for dial-in users to networks. Since then, it’s been expanded to use for other PPP (Point-to-Point Protocol) connections or for joining wireless networks. It can be used by ISPs (Internet Service Providers) to authenticate Internet users; it can also join remote users to internal enterprise networks with services not accessible over the Internet. It is a client-server protocol operating on UDP (User Datagram Protocol) port 1812, but probably doesn’t work in the way you think.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 

<h2>Program walk-through:</h2>

<p align="center">
From the start menu select "Server Manager": <br/>
<img src="https://i.postimg.cc/Y2gnVkdk/Screen-Shot-2022-08-25-at-11-28-28-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
On the Server Manager window select "Add Rolls and Features" and then click next three time  <br/>
<img src="https://i.postimg.cc/PxNGZcHJ/Screen-Shot-2022-08-25-at-11-30-08-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
In the role list check "Network Policy and Access Services":  <br/>
<img src="https://i.postimg.cc/j2wG3kM5/Screen-Shot-2022-08-25-at-11-33-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the pop up window select "Add Features" and then select next three times then click install: <br/>
<img src="https://i.postimg.cc/qBcJrNwv/Screen-Shot-2022-08-25-at-11-35-05-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Let the installation fully finish before continuing  <br/>
<img src="https://i.postimg.cc/ryC3hxyM/Screen-Shot-2022-08-25-at-11-37-17-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />


  

<br />
Let the installation fully finish before continuing  <br/>
<img src="https://i.postimg.cc/ryC3hxyM/Screen-Shot-2022-08-25-at-11-37-17-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
In the Server Manager window select "tools" in the top right corner then "Network Policy Server"  <br/>
<img src="https://i.postimg.cc/XY4VHdCb/Screen-Shot-2022-08-25-at-11-43-21-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />






<br />
In the Network Policy Server Window from the Standard Configuration List make sure that RADIUS server fro DIAL-Up or VPN Connections is selected  <br/>
<img src="https://i.postimg.cc/rwKhLYWC/Screen-Shot-2022-08-25-at-11-45-47-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Below the list select "Configure VPN or Dial-Up"  <br/>
<img src="https://i.postimg.cc/66MgJZgK/Screen-Shot-2022-08-25-at-11-49-24-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Below the list select "Configure VPN or Dial-Up"  <br/>
<img src="https://i.postimg.cc/66MgJZgK/Screen-Shot-2022-08-25-at-11-49-24-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Click "Virtual Private Network(VPN) Connections" then click next  <br/>
<img src="https://i.postimg.cc/TPQqLVrY/Screen-Shot-2022-08-25-at-11-51-30-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
In the "Configure VPN or Dial-Up" click add  <br/>
<img src="https://i.postimg.cc/jddW2pMN/Screen-Shot-2022-08-25-at-11-53-53-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
In the New RADIUS Client window type in the friendly name, Address, Shared secret, and confirm shared secret the click ok  <br/>
<img src="https://i.postimg.cc/0jQdxb3X/Screen-Shot-2022-08-26-at-12-01-42-AM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Click next in the window  <br/>
<img src="https://i.postimg.cc/yNrScs82/Screen-Shot-2022-08-26-at-12-06-12-AM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
In the Configure VPN or Dial-Up check the "Extensible Authentication Protocol" and uncheck MS-CHAPv2  <br/>
<img src="https://i.postimg.cc/4xNJR063/Screen-Shot-2022-08-26-at-12-12-54-AM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />







<br />
 From the type list select "Microsoft Protected EAP (PEAP)" and click next five times <br/>
<img src="https://i.postimg.cc/284K7dKF/Screen-Shot-2022-08-26-at-12-18-23-AM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />







<br />
 click "Finish" to accept all other defaults and create the policy <br/>
<img src="https://i.postimg.cc/ht5kvLZL/Screen-Shot-2022-08-26-at-12-38-51-AM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
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
