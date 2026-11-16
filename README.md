# Enterprise_Network
This is a home lab project to simulate security operations like red teaming and blue teaming. Log and Network packet analysis and integrate A.I..
Currently I have a splunk server deployed that is collecting logs from the splunk forwarder and sysmon on the windows client and server.

# Network Architecture
Built a network infrastructure that resembles a small enterprise environment, I started from the pfsense router using virtualbox, added network segmentations and firewall rules for security purposes and for allowing the windows server to connect to splunk that's on an ubuntu server in a DMZ.
pfsense interface
<img width="652" height="539" alt="image" src="https://github.com/user-attachments/assets/b446ed19-39f5-41af-a686-8c854dd6b10f" />

firewall
<img width="1273" height="703" alt="PfSense_Firewall_Rule_LAN" src="https://github.com/user-attachments/assets/38c6c7d6-a7ba-4a4a-90a9-4c3c79de4926" />

network diagram
<img width="575" height="509" alt="Network_Diagram" src="https://github.com/user-attachments/assets/4e73ea87-8e56-4f1f-b25f-e944a378bb49" />

# Enterprise Systems
I deployed virtual machines for an IT simulation and hardened LAN network and machines' security and policies. 
Windows Server 

Windows Server
Purpose: 
Identity Management 
Directory Services
DNS

Windows Client
Purpose: 
Domain User Workstation

Ubuntu Server
Purpose:
SOC Infrastructure
Splunk
Linux Administration

# SIEM Deployment
The set up I used for the SIEM server was on an ubuntu server in a DMZ network
Splunk Enterprise 
Web Interface
SSH Access
Receiving Port 9997
# Centralized Logging
Installed universal splunk forwarders, and sysmon for exprehensive logs indexed on splunk

# IDS/IPS 

# Attack Simulation
# Security Hardening
# SOC Operations
# AI Integration
