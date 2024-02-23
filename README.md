<h1>Bulid a SIEM system using Elasticsearch</h1>


<h2>Description</h2>
You'll create a home lab using Elastic's web portal and a Kali Linux VM to learn Elastic SIEM. Generate security events on Kali, forward data to SIEM, and analyze logs for insights.
<br />


<h2>Tools</h2>

- <b>Elastic Search</b>
- <b>Elastic Defender </b>
- <b>Kali linux VM</b>
- <b>Virtual machine or VMware</b>

<h2>Overview of tasks</h2>

- <b>Setup: You'll create a home lab environment using Elastic's web portal and a virtual machine (VM) running Kali Linux.
- Generating Security Events: On your Kali Linux VM, you'll simulate security events. This means creating situations that mimic real-world security threats, like attempted breaches or suspicious activities.
- Forwarding Data: You'll set up an agent on the Kali Linux VM to send the generated security event data to the Elastic SIEM. This is like installing a messenger to send the information securely to the SIEM platform.
- Query and Analysis: Once the data is in the SIEM, you'll use the Elastic web portal to query and analyze the logs. This involves asking specific questions about the data, like "show me all failed login attempts," and getting insights to understand potential security issues or patterns. <b>

<h2>Program walk-through:</h2>

<p align="center">
Step 1: Create an elastic account for free - https://cloud.elastic.co/registration  <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/e9cb4fff-abba-4853-a8a6-ff5abf29f099" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 2: Create Deployment <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/22f77919-6adf-4f4b-a343-f22c6c993729" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 3: After creating deployment download Kali VM - https://www.kali.org/get-kali/#kali-platforms
Add kali files on Virtual machine and the user name and password is kali. 
if you face any difficulty then search on youtube "how to setup kali vm on Virtual box"<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/0737987f-fba7-4d55-aa34-5ae594b73e3f" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 4: Putting agent on Kali VM to collect logs - 
        Go to elastic , Click on 3 lines , Click down "Add Integrations"<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/ffaf0b13-a130-47af-8353-7d694aa11dba" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Install Elastic: <br/>
<img src="https://i.imgur.com/xeb1h5f.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Reset Elastic password: <br/>
<img src="https://i.imgur.com/BwbA8AT.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Log into Elasticsearch: <br/>
<img src="https://i.imgur.com/9SnYdcr.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Launch Kibana: <br/>
<img src="https://i.imgur.com/rrhBGUV.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Configure Kibana with session token: <br/>
<img src="https://i.imgur.com/QjsSeiF.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Log into Kibana on port 5601: <br/>
<img src="https://i.imgur.com/vLGDfKd.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Edit Execution-Policy settings: <br/>
<img src="https://i.imgur.com/Qn7rcQv.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Install Winlogbeat: <br/>
<img src="https://i.imgur.com/d8d0gy1.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Edit Winlogbeat yaml config file: <br/>
<img src="https://i.imgur.com/o01NEXG.png" height="80%" width="80%" alt="SIEM System steps"/>
 <img src="https://i.imgur.com/4rTBi3b.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Install Elasticsearch SSL certificate: <br/>
<img src="https://i.imgur.com/pXiMoXc.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Launch Winlogbeat executable: <br/>
<img src="https://i.imgur.com/xrnFRMp.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Start Winlogbeat service: <br/>
<img src="https://i.imgur.com/x4KbjO0.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Final Product: <br/>
<img src="https://i.imgur.com/aY0Tvjh.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Using KQL to search for specific eventID’s: <br/>
<img src="https://i.imgur.com/m8RojNQ.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Using KQL to search for specific event ID’s coming from specific services: <br/>
<img src="https://i.imgur.com/SkvloZZ.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Creating Visualization Libraries using Kibana: <br/>
<img src="https://i.imgur.com/hpR6OH1.png" height="80%" width="80%" alt="SIEM System steps"/>
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

