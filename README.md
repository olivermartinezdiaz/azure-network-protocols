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

<img src="https://i.imgur.com/30ITQzN.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/RfL8MtI.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/Icvc4xc.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/B6AoSFL.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/h2YWUYx.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/BnVf1Ba.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/3Zm5TRc.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/wYzNYeE.png" alt="Traffic Examination"/>

Observe SSH Traffic 

<img src="https://i.imgur.com/FrMggXg.png" alt="Traffic Examination"/>
<img src="https://i.imgur.com/XA3jI7z.png" alt="Traffic Examination"/>

Observe DHCP Traffic 

<img src="https://i.imgur.com/rFgsuIZ.png" alt="Traffic Examination"/>

Observe DNS Traffic 

<img src="https://i.imgur.com/0efgBOc.png" alt="Traffic Examination"/>

Observe RDP Traffic 

<img src="https://i.imgur.com/NmTgdlu.png" alt="Traffic Examination"/>
