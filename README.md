# SSH-Honeypot-
Build a SSH Honeypot to lure attacker using Azure Vm and Splunk to understand real world attack

## Objective

The Honeypot project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs using Splunk, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used

-Microsoft Azure
-Cowrie Honeypot
-Splunk
-Powershell


## Steps
Step 1: Setting up Azure Virtual Machine

Created a Virutal Machine
<img width="1151" height="650" alt="Aazure VM" src="https://github.com/user-attachments/assets/43a6be19-63df-464a-b870-84c58572ad30" />

Configure NSG 

<img width="1031" height="373" alt="image" src="https://github.com/user-attachments/assets/2a8c3e76-fe02-467e-964b-b17b578f8ab7" />



Step 2: Secure SSH Key on Local Machine

Using icacls command to lock down private key before log into VM

<img width="700" height="250" alt="1" src="https://github.com/user-attachments/assets/b713e0fb-efb8-4a98-be48-b62cb900436d" />
<p></p>


Connect to Azure Virtual Machine

<img width="700" height="250" alt="2" src="https://github.com/user-attachments/assets/ec6f6fc0-7e50-409c-889f-109cf5996985" />
<p></p>

Step 3: Installation and Deployment of Honeypot

*Important: Before install cowrie honey make sure to switch to a decoy user  

Installing honeypot

<img width="609" height="376" alt="3" src="https://github.com/user-attachments/assets/32d0dee4-76f3-4e2a-97ef-bc41a138327a" />
<p></p>


Starting honeypot

<img width="619" height="147" alt="start" src="https://github.com/user-attachments/assets/3da2cbc4-6a6c-4436-a0bc-68462d26ca96" />
<p></p>


Configure the decoy server and telnet for better attack engagement

Change server naming for deception to make honeypot look like a high value target
<img width="570" height="363" alt="change server" src="https://github.com/user-attachments/assets/639b5764-ae79-4198-873b-ddf8e4d2db43" />
<p></p>

<p></p>
Enable telnet to expand attack

<img width="600" height="250" alt="telnet" src="https://github.com/user-attachments/assets/2379f212-3d77-4ed7-813a-b61db3889bfa" />
<p></p>

<p></p>


First 5 minutes of deployment

<img width="992" height="251" alt="break into honeypot" src="https://github.com/user-attachments/assets/6cd34735-2a1e-439d-930d-9930acc1ec9e" />
<p></p>

Step 4: Start splunk and collect log

Starting splunk service
<img width="1270" height="593" alt="image" src="https://github.com/user-attachments/assets/4982cb20-5a6d-47f8-b868-ffe76f341547" />
<p></p>

Virtualization of attack information
<img width="1264" height="557" alt="splunk1" src="https://github.com/user-attachments/assets/b8567106-9a32-4d96-91d0-c9a9acd260b8" />
<p></p>
<img width="1250" height="407" alt="splunk 2" src="https://github.com/user-attachments/assets/0fba43ab-8e2b-4236-8efc-0ab4ffc9c85a" />
<p></p>



