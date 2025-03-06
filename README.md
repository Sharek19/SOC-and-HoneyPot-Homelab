<h1>Implementing a SOC and Honeypot in Azure :honey_pot:</h1>


<h2>Description</h2>
In this lab, I built a home Security Operations Center (SOC) in Azure to monitor and analyze real-world cyber threats. The lab involved setting up an Azure Virtual Machine (VM) as a honeypot, collecting security logs, and using log analysis tools to detect and visualize attacks. By integrating Microsoft Sentinel, I was able to conduct threat investigations and create an interactive attack map to track hacker activity.





<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure</b> – Cloud environment for deploying security infrastructure.
- <b>Azure Virtual Machines (VMs)</b> – Hosted the honeypot system.
- <b>Remote Desktop Protocol (RDP)</b> – Connected to and managed the VM remotely.
- <b>Azure Log Analytics Workspace</b> – Centralized log storage and management.
- <b>Log Analytics Agent</b> – Forwarded logs from the VM to Log Analytics Workspace.
- <b>Microsoft Sentinel</b> – SIEM tool for analyzing security events and detecting threats.
- <b>Kusto Query Language (KQL)</b> – Used for querying and analyzing logs.
- <b>Geolocation Enrichment</b> – Mapped attacker IP addresses to physical locations.
- <b>Attack Map</b> – Visualized real-time threat activity.

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">

- Azure Virtual Machine Deployment: Create and configure a VM to simulate an exposed system.

![Virtual Machine](https://github.com/user-attachments/assets/b5546acd-8c3a-4307-bcdf-2bf671023807)


- Disabled the Firewall in order to set up the HoneyPot Trap

  
![image](https://github.com/user-attachments/assets/9106abce-1ee0-4da3-82a5-84ec6de61a36)


-Pinging the Virtual Machine.

![Ping VM](https://github.com/user-attachments/assets/137a39c6-6a3c-450e-8941-f1f300f071f5)

  
- Log Collection & Analysis: Set up Log Analytics Workspace to store and query security logs.

![Log Analytics Workspace](https://github.com/user-attachments/assets/f587502b-b4ad-46dc-9ea7-f2d2d006d808)


- Threat Investigation with KQL: Analyze failed login attempts and attack patterns using Kusto Query Language (KQL).

![Failed password logs](https://github.com/user-attachments/assets/92d5d80e-f0c1-4dd8-8bbb-61d2323f2225)


  
- SIEM Integration & Enrichment: Upload geolocation data to the SIEM for deeper threat insights.

![LOGS- GEOIP](https://github.com/user-attachments/assets/f3e26845-7ad1-4093-ab2a-744c6c648fc2)



- Attack Map Visualization: Build an interactive map to track hacker activity in real time. (The 5 US attempts were from me)

![image](https://github.com/user-attachments/assets/3b024be1-76b0-4525-b20c-5ded3fa2b906)



- Incident Detection & Response: Simulate real-world SOC operations by detecting and analyzing security events.
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
