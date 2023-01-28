<h1>Amazon Security Groups</h1>

<h2>Description</h2>
Project consists of creating security groups to govern ICMP and RDP access to AWS resources.
<br />


<h2>Utilities Used</h2>

- <b>Amazon Web Services</b>
- <b>RDP</b>
- Windows Server 2016

<h2>Creating an ICMP Security Group:</h2>
The Windows Server 2016 instance created previously is navigated to:<br/>
<img src="https://imagizer.imageshack.com/img924/9360/m7G1se.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The instance is right-clicked, and ran:<br/>
<img src="https://imagizer.imageshack.com/img922/7016/0jVRE9.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The security groups feature of EC2 is navigated:<br/>
<img src="https://imagizer.imageshack.com/img924/1369/FMdc0N.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Create security group is selected:<br/>
<img src="https://imagizer.imageshack.com/img924/8943/Iay4GI.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The security group is named and described. ICMP - IPv4 is selected from the dropdown with only my IP included:<br/>
<img src="https://imagizer.imageshack.com/img924/7889/0g53Se.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The actions dropdown is selected. Change security groups is opened:<br/>
<img src="https://imagizer.imageshack.com/img924/716/y7SJvq.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The associated security group for ICMP is added and saved:<br/>
<img src="https://imagizer.imageshack.com/img923/5492/yIO3Vn.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The instance is connected to via RDP:<br/>
<img src="https://imagizer.imageshack.com/img923/4476/w5zNDN.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The remote desktop file is downloaded and the Get password link is clicked:<br/>
<img src="https://imagizer.imageshack.com/img924/4602/LA1eGv.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The key pair created previously is uploaded, and the password is decrypted:<br/>
<img src="https://imagizer.imageshack.com/img922/7749/fKVJs6.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The session is then connected to using the decrypted password:<br/>
<img src="https://imagizer.imageshack.com/img924/3484/B0DAWC.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Yes is selected in the next window:<br/>
<img src="https://imagizer.imageshack.com/img922/9679/J0qZfr.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Successful connection to the server:<br/>
<img src="https://imagizer.imageshack.com/img924/2165/RHzlMP.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Creating an ICMPv4 Security Group:</h2>
The instance is attempting a ping from a host machine:<br/>
<img src="https://imagizer.imageshack.com/img922/8615/H6VZjm.png" alt="Disk Sanitization Steps"/>
<br />
<br />
While connected to the instance via RDP, windows firewall with advanced security is opened:<br/>
<img src="https://imagizer.imageshack.com/img923/5197/PadykY.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Inbound rules is opened and a new rule is created:<br/>
<img src="https://imagizer.imageshack.com/img922/760/3QuU8p.png" alt="Disk Sanitization Steps"/>
<br />
<br />
In rule type, custom is selected:<br/>
<img src="https://imagizer.imageshack.com/img923/801/FHTbgd.png" alt="Disk Sanitization Steps"/>
<br />
<br />
All programs is checked:<br/>
<img src="https://imagizer.imageshack.com/img922/161/hQ8T8I.png" alt="Disk Sanitization Steps"/>
<br />
<br />
ICMPv4 is selected from the dropdown:<br/>
<img src="https://imagizer.imageshack.com/img923/1153/Dkf9Xk.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Nothing is changed in scope:<br/>
<img src="https://imagizer.imageshack.com/img922/1623/g7zE8T.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Nothing is changed in action:<br/>
<img src="https://imagizer.imageshack.com/img924/4377/ZESMdX.png" alt="Disk Sanitization Steps"/>
<br />
<br />
Nothing is changed in profile:<br/>
<img src="https://imagizer.imageshack.com/img923/517/In8sxK.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The rule is named ICMPv4 allow and configuration is finished. A ping is now able to go through to the public IP:<br/>
<img src="https://imagizer.imageshack.com/img922/1293/E3qeN3.png" alt="Disk Sanitization Steps"/>
<br />
<br />
The session is disconnected, and the instance is stopped:<br/>
<img src="https://imagizer.imageshack.com/img924/6775/97gGs1.png" alt="Disk Sanitization Steps"/>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
