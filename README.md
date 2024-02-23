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
Step 5: Click on Elastic Defend <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/f108b2c8-04d7-410d-97f1-4c47e430c9d6" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 6: Click on Add <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/e72d5ee8-fbba-4059-b6f9-9bc1cdb91d28" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Configure whatever name you want to add then "save and continue": <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/458890a1-0234-41f0-9a0d-6a3922780406" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 7: Click on Add "Elastic agent to your host"<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/0a4143b6-9bc3-4085-afa4-3abed24fd3cb" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 8: Copy the Link🔗 (make sure your kali VM Running on background)<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/09621d0f-c941-4054-bd88-74949bf91b8f" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 9: Paste it on Kali VM and Press "Enter": <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/14fc0202-7094-4388-8514-5ea46b39b458" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 10: After Installed Successfully run this command - "sudo systemctl status elastic-agent.service" <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/3c67d0a7-0033-49bf-a0d4-3d91432ee323" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 11: Use Nmap on Kali VM to generate security events for testing.
       For install Run command - "sudo apt-get install nmap"
        After that run these 2 commands below 👇<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/4629611d-aa64-4bdc-97ba-b27b7f765265" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 12: Now that we've sent data from Kali VM to the SIEM, we can analyze and search through the logs in the SIEM to understand what's happening in our system.
        Go to Elastic >>> 3 lines >>> Observability >>> logs <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/c1d9feb1-9591-43e8-b5e2-7369670445cb" height="80%" width="80%" alt="SIEM System steps"/>
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

