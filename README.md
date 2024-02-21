<h1>Active Directory Lab</h1>


<h2>Description</h2>
This lab consists of going through the steps of creating an Active Directory home lab environment using Oracle Virtual Box. I did this in order to broaden my understanding of active directory and windows networking whilst hardening my knowledge on topics such as DHCP, NAT, and more. Starting from downloading Oracle Virtual Box and the associated ISOs for the VMs, I took a long journey constructing an actual network from the ground up consisting of a domain controller and an internal client that can both connect to the outside internet. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Oracle Virtual Box</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Servier 2019</b> 

<h2>Lab Screenshots</h2>

<p align="center">
Successfully downloaded Active Directory on VM meant to be domain controller(DC): <br/> <br />
<img src="https://i.imgur.com/0wXQmft.png" height="80%" width="80%" alt="Lab Screenshots"/>
<br />
<br />
Established a domain on domain controller as 'mydomain.com' : <br/> <br />
<img src="https://i.imgur.com/6w4dr7R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Successfully created admin user on domain controller VM: <br/> <br />
<img src="https://i.imgur.com/GI8fxl0.png" height="80%" width="80%" alt="Lab Screenshots"/>
<br />
<br />
Used PowerShell script to add aorund 1000 users to the established domain: <br/> <br />
<img src="https://i.imgur.com/NDzw66e.png" height="80%" width="80%" alt="Lab Screenshots"/>
<br />
<br />
Confirming DHCP on new Windows10 client VM(CLIENT1) recognizes DC as default gateway: <br/> <br />
<img src="https://i.imgur.com/rWikTaz.png" height="80%" width="80%" alt="Lab Screenshots"/>
<br />
<br />
Checking if internal client CLIENT1 has connection to internet via DC by pinging google.com : <br/> <br />
<img src="https://i.imgur.com/HFoPspR.png" height="80%" width="80%" alt="Lab Screenshots"/>
<br />
<br />
Observing new Address Lease given to CLIENT1 (DHCP within given range, client within established domain, lease expiration is set to 8 days) : <br/> <br />
<img src="https://i.imgur.com/fJIzfIa.png" height="80%" width="80%" alt="Lab Screenshots"/>
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
