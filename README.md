# SSH Honeypot Project
**Building an SSH Honeypot to lure attackers using Azure VM and Splunk to understand real-world attacks.**

## Objective
The Honeypot project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs using Splunk and created honeypot to mimic real world cyber attack. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned
- Cloud Security & Infrastrcuture hardening
- SIEM Data pipeline & analytics
- Honeypot Deception Deployment
- Cloud Firewall configuration
- Advanced linux command

### Tools Used
- Microsoft Azure
- Cowrie Honeypot
- Splunk
- PowerShell

## Steps

### Step 1: Setting up Azure Virtual Machine

**Create a Virtual Machine** 
<br>
<img width="1151" height="650" alt="Azure VM" src="https://github.com/user-attachments/assets/43a6be19-63df-464a-b870-84c58572ad30" />
<br><br>

**Configure Network Security Group (NSG)**
<br><br>
<img width="1031" height="373" alt="Configure NSG" src="https://github.com/user-attachments/assets/2a8c3e76-fe02-467e-964b-b17b578f8ab7" />
<br><br>

### Step 2: Secure SSH Key on Local Machine

**Lock down private key using `icacls` command**
<br>
<img width="700" height="250" alt="Locking down key" src="https://github.com/user-attachments/assets/b713e0fb-efb8-4a98-be48-b62cb900436d" />
<br><br>

**Connect to Azure Virtual Machine**
<br>
<img width="700" height="250" alt="Connect to VM" src="https://github.com/user-attachments/assets/ec6f6fc0-7e50-409c-889f-109cf5996985" />
<br><br>
### Step 3: Installation and Deployment of Honeypot
<br>
> **Important:** Before installing Cowrie, make sure to switch to a decoy user.

**Installing Honeypot**
<br>
<img width="609" height="376" alt="Install Honeypot" src="https://github.com/user-attachments/assets/32d0dee4-76f3-4e2a-97ef-bc41a138327a" />
<br><br>
**Starting Honeypot**
<br>
<img width="619" height="147" alt="Start Honeypot" src="https://github.com/user-attachments/assets/3da2cbc4-6a6c-4436-a0bc-68462d26ca96" />
<br><br>
**Configuration**

Changed server naming for deception to make the honeypot look like a high-value target.
<br>
<img width="570" height="363" alt="Change server name" src="https://github.com/user-attachments/assets/639b5764-ae79-4198-873b-ddf8e4d2db43" />
<br><br>
Enabled Telnet to expand attack surface.
<br>
<img width="600" height="250" alt="Enable Telnet" src="https://github.com/user-attachments/assets/2379f212-3d77-4ed7-813a-b61db3889bfa" />
<br><br>

**Result: First 5 minutes of deployment**
<br>
<img width="992" height="251" alt="Break into honeypot" src="https://github.com/user-attachments/assets/6cd34735-2a1e-439d-930d-9930acc1ec9e" />
<br><br>
### Step 4: Start Splunk and Collect Logs

**Starting Splunk Service**
<br>
<img width="1270" height="593" alt="Start Splunk" src="https://github.com/user-attachments/assets/4982cb20-5a6d-47f8-b868-ffe76f341547" />
<br><br>
**Visualization of Attack Information**
<br>
<img width="1264" height="557" alt="Splunk Dashboard 1" src="https://github.com/user-attachments/assets/b8567106-9a32-4d96-91d0-c9a9acd260b8" />
<br><br>
<img width="1250" height="407" alt="Splunk Dashboard 2" src="https://github.com/user-attachments/assets/0fba43ab-8e2b-4236-8efc-0ab4ffc9c85a" />
<br><br>
