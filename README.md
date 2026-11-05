 # 🛡️ Network-Security-Lab-Wireshark-Packet-Analysis

---

<p align="center">
  <b>Task:</b> Network Security & Traffic Analysis
  <br>
  <b>Focus:</b> Wireshark Packet Inspection
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Network%20Security-red">
  <img src="https://img.shields.io/badge/Tool-Wireshark-blue">
  <img src="https://img.shields.io/badge/Focus-Packet%20Analysis-green">
  <img src="https://img.shields.io/badge/Skill-Traffic%20Monitoring-orange">
  <img src="https://img.shields.io/badge/Topic-Intrusion%20Detection-purple">
  <img src="https://img.shields.io/badge/Field-SOC%20Analysis-black">
</p>

---

## 📝 Executive Overview

**Scenario.** You are a SOC analyst. A staff member has reported unusual traffic to your company's web server. Capture the packets and analyze them in Wireshark. Find out what type of attack this is and what the attacker's IP address is.

---

## 🎯 Project Objectives

- Capture network traffic for investigation.
- Analyze suspicious packets using Wireshark.
- Identify unusual network communication patterns.
- Determine the type of attack.
- Identify the attacker's IP address.
- Document findings and investigation results.

---
## Phase 1:
Open the `Wireshark` and click here you can see the traffic here going through the network.

<img width="626" height="372" alt="image" src="https://github.com/user-attachments/assets/3238e8a8-d2d6-44bb-9f33-4080a6e4d380" />

---
## Phase 2:
Sign in to the Windows PC and capture the network traffic. How many packets did Wireshark capture?
Total Packets captured `309`

<img width="692" height="241" alt="image" src="https://github.com/user-attachments/assets/d4db35c1-b2b8-43fb-8449-3aca447df216" />

---
## Phase 3:
Most of this traffic is normal. Show only the packets that start a TCP connection (the SYN flag is set). How many packets are displayed? So we have total of Syn packets capture is `73` by using this filter `tcp.flags.syn`

<img width="692" height="250" alt="image" src="https://github.com/user-attachments/assets/bd0fefbf-6a0d-467b-a784-bf13cd23a757" />

---
## Phase 4:
Most PCs send only one or two of these packets. One IP address sends a long block of them, one after another. What is the attacker’s IP address? So this looks suspicious so we will look for the atacker ip add `192.168.10.66`

<img width="692" height="247" alt="image" src="https://github.com/user-attachments/assets/ca0414d3-61b4-41ab-aafb-3c50d5bc62e4" />

---
## Phase 5:
Which IP address is the target of the attacker’s packets? target ip add is `192.168.10.20`

<img width="691" height="247" alt="image" src="https://github.com/user-attachments/assets/fd064345-61b9-41b3-a83e-d74684f814f3" />

---
## Phase 6:
Look at the attacker’s packets in the Info column. One port number is the same in every packet. What is it? If we look at the attacker packets the port number is `52311`

<img width="692" height="263" alt="image" src="https://github.com/user-attachments/assets/0c422276-e4f9-4351-a6f1-48f3817af96d" />


