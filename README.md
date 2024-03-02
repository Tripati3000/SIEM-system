# Building a SIEM system using Elasticsearch 🛡️💻

<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/97d1f0f9-84cd-41e6-939a-419b7e8ddfa8" height="80%" width="80%" alt="SIEM System steps"/>



# What is a SIEM ?🤔
SIEM stands for Security Information and Event Management. It's like a digital security guard for computer systems. It collects and analyzes data from various sources like logs and sensors to detect and respond to security threats and incidents in real-time. Think of it as a tool that helps organizations monitor, detect, and investigate potential security breaches or unusual activities within their networks.

# Description
You'll create a home lab using Elastic's web portal and a Kali Linux VM to learn Elastic SIEM. Generate security events on Kali, forward data to SIEM, and analyze logs for insights.
<br />


# Tools

- <b>Elastic Search</b>
- <b>Elastic Defender </b>
- <b>Kali linux VM</b>
- <b>Virtual machine or VMware</b>

# Overview of tasks

- <b>Setup: You'll create a home lab environment using Elastic's web portal and a virtual machine (VM) running Kali Linux.
- Generating Security Events: On your Kali Linux VM, you'll simulate security events. This means creating situations that mimic real-world security threats, like attempted breaches or suspicious activities.
- Forwarding Data: You'll set up an agent on the Kali Linux VM to send the generated security event data to the Elastic SIEM. This is like installing a messenger to send the information securely to the SIEM platform.
- Query and Analysis: Once the data is in the SIEM, you'll use the Elastic web portal to query and analyze the logs. This involves asking specific questions about the data, like "show me all failed login attempts," and getting insights to understand potential security issues or patterns. <b>

# walkthrough:

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
 <img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/8da0754e-6e90-4cd5-8568-90ae886593d2" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 13: >> Enter search query in the bar.
         >> Click "Search".
         >> Results show below.
         >> Click dots for more details.
         Analyzing events helps understand security incidents.
 <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/af216f55-315b-4b6c-9642-19d45ad7f78a" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 14: Use visualizations and dashboards to analyze logs for patterns or anomalies. For instance, create a dashboard showing security event counts over time. 
        Go to elastic >> 3 lines >> Analytic >> dashboard >> create visualization 👍<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/2e75384a-2f40-433b-8995-13ded5f45b9b" height="80%" width="80%" alt="SIEM System steps"/> 
  <img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/bb43e3ad-dd3d-4edc-bfe2-d6334ca005d2" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 15: Select Area <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/bd46444b-86d7-4876-a898-4007bee0df7f" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 16: Click Horizantal axis and select "Timestamp" and for Vertical axis select "Count".
        So here,"Count" for the number of events and "Timestamp" for the time axis to show event counts over time.
        <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/53309ed9-29b9-4102-be10-9a79d4ede322" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 17: After that Save it 😄 <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/db53d9e0-063d-4857-b06a-f20fa6b42c2e" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 18: Create Alert (importamt)✅ 
        >>> Go to Alerts
        >>> Click 'Manage rules' at top right corner.
        >>> Click 'Create new rules'
        >>> On 'define rule' section click 'Custum query'<br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/fb4329e2-a92f-4c41-a6be-1e46dee74d46" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Step 19: Search >>> event.action:"nmap-scan" on Custum query.
        on about rule section give your rule name or description like (nmap detection)
        and Choose how serious the alert is, so you know which ones need immediate attention. Leave all other settings as they are and then click "Continue." <br/>
<img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/10a5df3d-773a-4843-a1a0-9028797fb364" height="80%" width="80%" alt="SIEM System steps"/>
        <img src="https://github.com/Tripati3000/SIEM-system/assets/160244601/deaba781-a085-4f12-8803-4122f65a85ab" height="80%" width="80%" alt="SIEM System steps"/>
        
Step 20:
        
1. After setting up Custum query Go to the "Actions" section.
        
2. Choose what action you want to happen when the rule activates: send an email notification, create a Slack message, or trigger a custom webhook.

3. Click on the "Create and enable rule" button to set up the alert.
 
5. Once the alert is created, it will monitor your logs for Nmap scan events.

6. If an Nmap scan event is detected, the alert will be triggered, and the action you selected will be executed.
 
9. To manage your alerts, go to the "Alerts" section under "Security."

        
# Conclusion 👍
        
We built a home lab using Elastic SIEM and a Kali VM. We connected the Kali VM to the SIEM using Elastic Beats agent to send data. Then, we created security events on the Kali VM using Nmap. We checked and studied these logs in the SIEM using the Elastic web interface. Additionally, we made a dashboard to display security events visually. Finally, we set up an alert to catch security events as they happen.

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>

