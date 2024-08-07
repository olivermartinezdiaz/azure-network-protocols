<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />

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

- Create Resource Groups and Virtual Machines
- Install & Run Wireshark
- Observe ICMP Traffic
- Observe SSH Traffic
- Observe DHCP Traffic
- Observe RDP Traffic

<h2>Actions and Observations</h2>

Create Resource Groups and Virtual Machines 

<img src="https://i.imgur.com/nADicjc.png" alt="Traffic Examination"/>

Install Wireshark in Virtual Machine 1

<img src="https://i.imgur.com/InQJNmH.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/6vUDrp7.png" alt="Traffic Examination"/>

Open Wireshark Click Blue fin to observe ICMP traffic

<img src="https://i.imgur.com/bAgV6I4.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/1q3B0Jx.png" alt="Traffic Examination"/>

Observe ICMP Traffic 
Type ICMP in the filter bar to filter only ICMP traffic 

<img src="https://i.imgur.com/30ITQzN.png" alt="Traffic Examination"/>

Ping VM-2 Using its private IP address from Azure.
<img src="https://i.imgur.com/RfL8MtI.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/Icvc4xc.png" alt="Traffic Examination"/>

From Windows 10 virtual machine, open PowerShell and ping the website WWW.google.com and observe the traffic in Wireshark. 

<img src="https://i.imgur.com/B6AoSFL.png" alt="Traffic Examination"/>

Send a nonstop ping to VM-2 with the command ping -t
<img src="https://i.imgur.com/h2YWUYx.png" alt="Traffic Examination"/>

In Azure go into VM-2 network security group and add an inbound rule to stop ICMP traffic.
<img src="https://i.imgur.com/BnVf1Ba.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/3Zm5TRc.png" alt="Traffic Examination"/>

Delete the inbound rule or simply allow the inbound rule to receive ICMP traffic (control+C to stop non-stop packets)
<img src="https://i.imgur.com/wYzNYeE.png" alt="Traffic Examination"/>

Observe SSH Traffic 
From the Windows 10 virtual machine, connect to VM2 virtual machine using SSH via PowerShell. 
Using Powershell type SSH username@ Vm2 Private IP address and hit enter. Type in the login password(note password wont show)
<img src="https://i.imgur.com/FrMggXg.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/XA3jI7z.png" alt="Traffic Examination"/>

Observe DHCP Traffic 
Type the command ipconfig/renew the VM will receive a new IP address Observe the traffic in WireShark.(The VM may restart to receive IP address)

<img src="https://i.imgur.com/rFgsuIZ.png" alt="Traffic Examination"/>

Observe DNS Traffic 
In Powershell type the command "nslookup" www.google.com. Observe the IP address and DNS in Wireshark
<img src="https://i.imgur.com/0efgBOc.png" alt="Traffic Examination"/>

Observe RDP Traffic 

<img src="https://i.imgur.com/NmTgdlu.png" alt="Traffic Examination"/>
