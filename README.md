# Enterprise_Network
This is a home lab project to simulate security operations like red teaming and blue teaming. Log and Network packet analysis and integrate A.I..
Currently I have a splunk server deployed that is collecting logs from the splunk forwarder and sysmon on the windows client and server.

# Network Architecture
Built a network infrastructure that resembles a small enterprise environment, I started from the pfsense router using virtualbox, added network segmentations and firewall rules for security purposes and for allowing the windows server to connect to splunk that's on an ubuntu server in a DMZ.

network diagram
A logical network architecture diagram to display my home lab set up.
<img width="575" height="509" alt="Network_Diagram" src="https://github.com/user-attachments/assets/4e73ea87-8e56-4f1f-b25f-e944a378bb49" />

pfsense interface
I started with a pfsense router and segmented the network into WAN, LAN and a DMZ.
<img width="652" height="539" alt="image" src="https://github.com/user-attachments/assets/b446ed19-39f5-41af-a686-8c854dd6b10f" />

firewall
Created firewall rules for network communication and network security

WAN Firewall Rules
<img width="1280" height="787" alt="PfSense_WAN_Interface" src="https://github.com/user-attachments/assets/b2fbd5ed-5c81-44ba-9ced-17567006b258" />

LAN Firewall Rules
<img width="1273" height="703" alt="PfSense_Firewall_Rule_LAN" src="https://github.com/user-attachments/assets/38c6c7d6-a7ba-4a4a-90a9-4c3c79de4926" />

DMZ Firewall Rules
<img width="636" height="701" alt="DMZ_FirewallRules" src="https://github.com/user-attachments/assets/5997191d-b2de-43ae-b6b7-5dad1a73bc46" />

DMZ Port Forwarding Rules 
<img width="637" height="738" alt="DMZ_FireWall_Port_Forwarding" src="https://github.com/user-attachments/assets/f39a1686-5a83-49f8-85af-a4ef71db5aaa" />

Testing DMZ  firewall rules
<img width="394" height="153" alt="DMZ_Firewall_Rule_Test" src="https://github.com/user-attachments/assets/d3f53a61-68a0-4934-b9b5-34fa21005695" />

# Enterprise Systems
I deployed virtual machines for an IT simulation and hardened LAN network and machines' security and policies.

Windows Server Dashboard
<img width="641" height="673" alt="image" src="https://github.com/user-attachments/assets/660b9c99-b4b3-41f1-b785-aa3735ff8d4c" />

Active Directory Users and Computers
<img width="302" height="132" alt="image" src="https://github.com/user-attachments/assets/5b619fca-3f0c-4833-85a9-b8957d0003f1" />

DNS Forwarders
<img width="467" height="480" alt="image" src="https://github.com/user-attachments/assets/4762824e-d401-4665-8fbb-1c8d5036eced" />


Purpose: 
Identity Management 
Directory Services
DNS

Windows Client
Purpose: 
Windows Client
<img width="253" height="214" alt="image" src="https://github.com/user-attachments/assets/d19c826a-7a29-44ca-a690-12174d935a81" />

Security Policy
<img width="623" height="359" alt="image" src="https://github.com/user-attachments/assets/02c99e4b-39c4-42b3-ba36-ba290b3040f8" />

Domain User Workstation

Ubuntu Server
Purpose:
SOC Infrastructure
Splunk
Linux Administration

# SIEM Deployment
The set up I used for the SIEM server was on an ubuntu server in a DMZ network
Splunk Enterprise 

Splunk Web Interface Accessed through windows client
<img width="996" height="652" alt="Splunk-Dashboard" src="https://github.com/user-attachments/assets/82fe7340-bf92-4f46-897c-2b790d95c8ad" />

Receiving Port 9997
<img width="637" height="464" alt="Splunk_Receiving_Conf_WEBGUI" src="https://github.com/user-attachments/assets/2846a9f3-6e3f-43a9-9746-1c56e847ecc4" />

Windows Splunk Forwarder Configuration
<img width="1279" height="712" alt="splunk_forwarders_confpng" src="https://github.com/user-attachments/assets/b7550395-8bca-4998-812a-f848b92b764f" />

Troubleshooting Errors

Error Downloading Splunk package
write: error, Not enough space on my virtual disk.
<img width="1280" height="524" alt="dpkg-error" src="https://github.com/user-attachments/assets/2aa119aa-d061-4305-afc5-b5874858cb56" />

Expanded my storage
<img width="638" height="538" alt="resize" src="https://github.com/user-attachments/assets/bf855a4d-55d4-4ee1-bbe6-a988060493df" />

Expanded my file system
<img width="638" height="242" alt="grow_filesystem" src="https://github.com/user-attachments/assets/c21ab08f-9805-4efe-89b3-fec0d4e96400" />

Splunk Start Error: Permission Denied
<img width="644" height="662" alt="splunk_start_error" src="https://github.com/user-attachments/assets/c11bd5f4-7347-4200-b3f6-21abb791754f" />
Meaning there was something wrong with user permissions like read, write and execute
Fix: Change user permissions for the file
<img width="636" height="90" alt="chown" src="https://github.com/user-attachments/assets/61e0efbc-a3b0-4ebb-ba3d-c4e797f6d2c2" />


# Centralized Logging
Installed universal splunk forwarders, and sysmon for exprehensive logs indexed on splunk

# IDS/IPS 

# Attack Simulation
# Security Hardening
# SOC Operations
# AI Integration
