# 30-Day-MyDFIR-Elastic-Challenge

30-Day MyDFIR Elastic Challenge

Overview

This repository documents my 30-Day MyDFIR Elastic Challenge, a hands-on SOC and DFIR lab project focused on deploying, operating, and investigating security events using the Elastic Stack (Elasticsearch, Logstash, Kibana). The project simulates real-world enterprise monitoring by combining endpoint telemetry, attack simulation, alerting, dashboards, and incident workflow integration.
This challenge emphasizes practical detection engineering, incident investigation, and SOC workflows, rather than theory alone.

Objectives

•	Deploy a full Elastic Stack in a cloud-based lab

•	Centralize log ingestion from Windows and Linux endpoints

•	Implement endpoint telemetry using Sysmon and Elastic Agent

•	Simulate real-world attacks (Brute Force, RDP abuse, C2)

•	Build alerts and dashboards for SOC monitoring

•	Perform DFIR-style investigations

•	Integrate alerting with a ticketing system

Lab Architecture
Core Components:

•	Elasticsearch

•	Logstash

•	Kibana

•	Elastic Agent & Fleet Server

•	Sysmon (Windows telemetry)

•	Mythic C2 Framework

•	OS Ticket (Incident management)


Endpoints:

•	Windows Server 2022

•	Ubuntu Server 24.04

•	Kali Linux (attacker system)

Infrastructure:


•	Cloud-hosted virtual machines (Vultr)


Tools & Technologies

•	Elastic Stack (ELK)

•	Elastic Defend

•	Sysmon

•	Mythic C2

•	OS Ticket

•	Kali Linux

•	Ubuntu Server 24.04

•	Windows Server 2022

•	FreeRDP

•	Gitbash 


30-Day Challenge Breakdown

Day 1–4: Elastic Stack Foundations

•	Logical architecture design

•	Introduction to Elasticsearch, Logstash, and Kibana

•	Elasticsearch and Kibana setup

Day 5–10: Endpoint Telemetry

•	Windows Server 2022 installation

•	Elastic Agent & Fleet Server deployment

•	Sysmon installation and configuration

•	Log ingestion into Elasticsearch

Day 11–17: Detection & Visualization

•	Brute force attack concepts

•	Ubuntu Server deployment

•	Elastic Agent on Linux

•	Creation of Kibana alerts and dashboards

•	RDP security overview

Day 18–22: Command and Control

•	C2 fundamentals

•	Attack flow diagram

•	Mythic server and agent deployment

•	C2 alerting and dashboards

Day 23–25: SOC Workflow Integration

•	Ticketing system concepts

•	OS Ticket deployment

•	Integration of OS Ticket with Elastic alerts

Day 26–28: Incident Investigations

•	SSH brute force attack investigation

•	RDP brute force attack investigation

•	Mythic C2 agent investigation

Day 29–30: Endpoint Protection & Optimization

•	Elastic Defend installation

•	Troubleshooting and environment optimization

Screenshots & Evidence

The following figures document key stages of the lab implementation, attack simulation, detection, and investigation. All screenshots were captured from the live lab environment.

Figure 1: Vultr cloud dashboard showing running lab infrastructure (ELK server, Fleet Server, Linux endpoint, Windows Server, Mythic server).

Figure 2: Sysmon installation and configuration

Figure 3: Kibana dashboard showing SSH authentication failures and Successful SSH Authentication 

Figure 4: Kibana dashboard showing RDP authentication failures and Successful RDP Authentication 

Figure 5: Elastic Security alert triggered for suspected SSH brute-force activity and suspected RDP brute-force activity.

Figure 6: Mythic C2 dashboard showing active callbacks from compromised Windows Server endpoint.

Figure 7: Kali Linux (VirtualBox) initiating RDP connection to Windows Server using FreeRDP during attack

Detection Use Cases Implemented

•	SSH Brute Force Detection

•	RDP Brute Force Detection

•	Command-and-Control Beaconing

•	Suspicious Authentication Patterns

•	Endpoint Process Execution Monitoring

Key Skills Demonstrated

•	SOC monitoring and alerting

•	Detection engineering

•	DFIR investigation methodology

•	Endpoint telemetry analysis

•	C2 behavior analysis

•	Incident ticketing workflows

•	Cloud-based SOC lab deployment

MITRE ATT&CK Coverage 

•	T1110 – Brute Force

•	T1021 – Remote Services (RDP, SSH)

•	T1059 – Command and Scripting Interpreter

•	T1071 – Application Layer Protocol (C2)

•	T1105 – Ingress Tool Transfer


Lessons Learned

•	Importance of telemetry quality over alert quantity

•	Value of centralized agent management via Fleet

•	Challenges in tuning alerts to reduce false positives

•	Practical visibility into attacker behavior through C2 simulation

Disclaimer
This project was conducted strictly for educational and defensive security purposes within a controlled lab environment. No unauthorized systems were accessed.


 <img width="940" height="312" alt="image" src="https://github.com/user-attachments/assets/15904dba-1c9d-4c19-88fb-63b4de6feeec" />
Figure 1


 <img width="940" height="356" alt="image" src="https://github.com/user-attachments/assets/b8b88268-edc7-4cb7-9552-ca08718dab2b" />
Figure 2


<img width="940" height="418" alt="image" src="https://github.com/user-attachments/assets/b85355ef-ef5f-4310-8e4c-30a87f544f97" />
Figure 3


 <img width="940" height="430" alt="image" src="https://github.com/user-attachments/assets/050a1721-7a9a-4e20-9b98-1d1dbbb9b9e9" />
Figure 4


<img width="940" height="361" alt="image" src="https://github.com/user-attachments/assets/fee67724-2160-4fab-accc-3726c26a3f2a" />
Figure 5


 <img width="940" height="469" alt="image" src="https://github.com/user-attachments/assets/614519a0-d234-4780-8078-665e1e8892f7" />
Figure 6


 <img width="940" height="499" alt="image" src="https://github.com/user-attachments/assets/2bd8350d-ecf3-46d8-9a2a-e12900bc5766" />
Figure 7

