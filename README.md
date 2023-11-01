# Simple Reverse Shell with NetCat


<h3>Description</h3>
<h1></h1>
<b>Using NetCat to create a Reverse Shell and obtain access to target machine.
</b>
<br />
<br />
To emulate the desired environments, I employed the use of two virtual machines using linode. Within this setup, I utilized the NetCat command to establish a reverse shell. One of these virtual machines functioned as the host, taking on the role of the attacker, while the other ran Kali Linux and assumed the role of the target. Initially, the host/attacker machine awaited incoming signals. Subsequently, the target machine executed a code or command embedded within a payload, granting the attacker unrestricted access to the target device. The primary objective was to successfully establish this connection, ultimately leading to complete control over the target. This exemplifies a basic illustration of the functionality of reverse shells. I may delve further into the topic of payloads in this repository at a later time.
<br />
<br />


<p align="center">
<img src="https://i.imgur.com/5FgKk4H.png" height="85%" width="85%" alt="Linodes Vm's"/>
</p>

<h2>Login to host and send out signal</h2>
<b>
</b>

When accessing the host system established on Linode, we initiate the transmission of the receiving signal. To clarify, we employ the NetCat command, where "nc" represents NetCat and "lnvp" is an abbreviation for "listen, numeric, verbose, and port." NetCat is configured to actively listen for incoming signals, and it utilizes the specified IP address and open port. Its primary function is to translate these signals into human-readable data, facilitating communication and understanding between the involved systems.
<br />
<br />


<p align="center">
<img src="https://i.imgur.com/EB8E55f.png" height="85%" width="85%" alt="Host"/>
</p>
<p align="center">
<img src="https://i.imgur.com/NvqtiVm.png" height="85%" width="85%" alt="Receive"/>
</p>

<h2>Target Machine</h2>
<b>(skipping payload)
</b>
<br />
<br />
In the context of exploiting a target system, various methods, known as "payloads," can be employed to automate the process of providing access to the attacker's machine. These payloads are designed to be covert and often involve social engineering, software vulnerabilities, or other means of bypassing security mechanisms to execute malicious code on the target system.
<br />
<br />


<p align="center">
<img src="https://i.imgur.com/Jg0E9Xz.png" height="85%" width="85%" alt="connectatmpt"/>
</p>
<p align="center">
<img src="https://i.imgur.com/BZ4cJDe.png" height="85%" width="85%" alt="connectsuccess"/>
</p>



<h2>Languages Used</h2>

- <b>Batch Languages



<h2>Access Proof</h2>
<b>Upon the successful establishment of the reverse shell connection, the attacker gains a significant level of control over the target device. This control extends beyond mere access; it encompasses the ability to execute various commands and operations on the target system. With this control, the attacker can explore the device's file system, access sensitive data, manipulate configurations, and even install or uninstall software as needed. 
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/yGwoiEk.png" height="85%" width="85%" alt="Map Data"/>
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
