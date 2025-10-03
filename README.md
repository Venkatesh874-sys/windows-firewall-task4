# windows-firewall-task4
Configuration and testing of Windows Defender Firewall rules to block insecure traffic (Telnet port 23), verify rule effectiveness, and document results for cybersecurity internship Task 4
# 🔐 Cybersecurity Internship – Task 4: Windows Firewall Configuration

## 🧭 Objective
Configure and test basic firewall rules on Windows to block insecure traffic and demonstrate network protection using Telnet.

---

## 🛠️ Tools Used
- Windows Defender Firewall with Advanced Security  
- Telnet Client (for testing)  
- Command Prompt  
- Screenshot tool

---

## 📌 Steps Performed

### Step 1: Open Firewall Configuration
- Accessed via `wf.msc` or Control Panel → System and Security → Windows Defender Firewall → Advanced Settings.
- 
<img width="1920" height="1020" alt="2025-10-03" src="https://github.com/user-attachments/assets/90a05085-76e6-42de-b2c6-472a80e8dbae" />

### Step 2: Create Inbound Rule to Block Port 23 (Telnet)
- Protocol: TCP  
- Port: 23  
- Action: Block the connection  
- Profile: Domain, Private, Public  
- Rule Name: `Block Telnet Port 23`
<img width="892" height="726" alt="2025-10-03 (1)" src="https://github.com/user-attachments/assets/cc07365e-3527-4a61-83da-2de5fea78fe4" />



### Step 3: Enable Telnet Client
- Installed via Windows Features (`optionalfeatures`)  
- Verified using: `telnet localhost 23`
<img width="1920" height="1020" alt="2025-10-03 (9)" src="https://github.com/user-attachments/assets/7a88f6b4-c749-4a52-90c4-1ddd6197ebb2" />


### Step 4: Test the Rule
- Ran: `telnet localhost 23`  
- Result: `Connect failed` – confirms port 23 was successfully blocked
<img width="892" height="726" alt="2025-10-03 (8)" src="https://github.com/user-attachments/assets/daf78c2e-dd45-41a7-9f77-d2ac94a3618c" />


### Step 5: Delete the Rule
- Removed `Block Telnet Port 23` from Inbound Rules

<img width="402" height="214" alt="2025-10-03 (5)" src="https://github.com/user-attachments/assets/38e083a8-7cff-4016-ac64-e89e0d21ea16" />

### Step 6: Remove Telnet Client
- Unchecked Telnet Client in Windows Features to restore system security

## 📚 What I Learned
- How to configure and manage firewall rules using Windows GUI  
- Importance of blocking insecure ports like Telnet  
- How firewalls filter traffic based on protocol, port, and direction  
- Real-world testing using Telnet to validate firewall behavior  
- Professional documentation and troubleshooting skills

ture

