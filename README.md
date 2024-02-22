<h1>Bulid a SIEM system using Elasticsearch</h1>


<h2>Description</h2>
This task involves setting up a Windows system to incorporate improved logging for user login/logout events, user process launches, and network activity. We will establish a SIEM solution using an Elasticsearch stack, enabling the ingestion, visualization, and querying of log data sources.
<br />


<h2>Tools</h2>

- <b>Elastic Search</b>
- <b>Elastic Kibana </b>
- <b>Winlogbeat</b>
- <b>PowerShell</b>
- <b>KQL</b>
- <b>Sysmon</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)

<h2>Program walk-through:</h2>

<p align="center">
Enable Local Security Policy: (only required on home versions) <br/>
<img src="https://i.imgur.com/YTMkRzT.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Enable Success and Failure Auditing: <br/>
<img src="https://i.imgur.com/mXVy0M8.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Enable Windows Firewall logging: <br/>
<img src="https://imgur.com/CWzrhND.png" height="80%" width="80%" alt="SIEM System steps"/>
<br />
<br />
Enable Sysmon and import configuration file: <br/>
<img src="https://i.imgur.com/rw9b5xn.png" height="80%" width="80%" alt="SIEM System steps"/>
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

