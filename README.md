# Intrusion_Detection_System

## 1. Introduction

Computer networks have become an integral part of our lives. They are used to store and transmit sensitive information,
such as personal data, and financial records. As a result, computer networks are vulnerable to various security threats, such
as hacking, and data theft. **Intrusion Detection Systems** (IDS) are essential tools for detecting and preventing these threats.
The main purpose of an IDS is to monitor network traffic, identify potential security threats, and alert administrators to act.
IDSs use various techniques like anomaly detection, and machine learning algorithms to detect malicious activity. Python
Libraries like pandas, tkinter, scapy and matplotlib are used. When threat is detected, the IDS can trigger response
mechanisms, such as **blocking traffic or alerting security personnel**. Various components of the system, including the sensors, 
analysis engine, response mechanisms, and management interface are implemented in code.

## 2. Methodologies:

  **2.1 System Architecture**

  1. Sensors: Software that monitors network traffic and collects data for analysis. In this regard Wireshark is used to capture
packets.

  2. Analysis engine: This component is responsible for processing and analyzing the data collected by the sensors. The
analysis engine can use machine learning algorithms to identify potential threats. The graphs are made in this regard so that
one can see the types of the attacks, who attacked like their source IP and number of attacks by specific IP’s.

  3. Response mechanism: Once a threat is detected, it has a mechanism to respond and mitigate the threat. It involves sending
an alert to ADMIN via email and blocking IP addresses.

  4. Management interface: It has a user interface that allows administrators to monitor the system and view the results of the
attacks.

  **2.2 Sensor Selection and Configuration**
  
  Wireshark file is used as a sensor which is used to capture the packets. The Wireshark file is saved and used for analysis.

![wire_pic](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/9428cf7f-7876-4640-bfe7-071667e221da)
  
  **2.3 Rules and Signatures Development**

The SSH rule is designed to detect potential brute force attacks on SSH servers. Brute force attacks are often used by
attackers to guess username and password combinations to gain unauthorized access to a system.

While the ARP rule is designed to detect potential ARP spoofing attacks. ARP spoofing is a technique used by attackers to
link their own MAC addresses with the IP address of another device on a local network. This can be used to redirect network
traffic or to conduct man-in-the-middle attacks.

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/6cc3c482-eeed-49ca-b67c-abb652ea7233)


  **2.4 Analysis Engine Development**

For analysis, graphs are used like bar, pie and histogram. The protocols, IP addresses and attack types like
probe, dos, etc are analyzed as shown in the figures:

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/96a9676b-adff-4f66-bcc3-4a9e411ed6fa)

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/f42bd322-75ae-4e91-94ef-85839955fdd8)

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/6cb64162-27fc-4d2a-9197-74485e775bed)

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/a985afd3-213e-42fa-b100-0ae3e4a6d4af)

  **2.5 Response Mechanism**
When the threat is identified from specific IP addresses then those were blocked, and the email was sent to identified
threats.

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/f43883a6-e0a9-48b7-86e1-be292650a51a)

_Email Sent and received_

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/47ae280e-f460-40af-ac70-963706019792)


![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/76f57437-6d90-4313-bb04-7298625045a6)

  **2.6 Management Interface**

Interface allows administrators to monitor the system and respond to security threats.
The Wireshark.pcapng file was selected and threats were detected, if threats exceeded the threshold from the specific IP
addresses, then it shows the FLOOD attack also shows that email is sent and IP has been blocked as show in figures.

![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/e4987247-aa40-48ea-aa18-bf4c864dd55c)


![image](https://github.com/MukandKrishna/Intrusion_Detection_System/assets/89685704/ed16647c-7eed-4f5b-8017-039a6ad05d79)

  **2.7 Testing and Validation**
  
Detection System is tested using another Wireshark file too for testing purpose to ensure that system is working fine.

  ## 3. Conclusion
  
In conclusion, the testing of Intrusion Detection Systems is important to ensure computer networks security. By
implementing effective IDS solutions, organizations can protect their networks from potential security threats and ensure
the confidentiality, and integrity of their data.






