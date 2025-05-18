### <br>### SOC Lab - Reverse Shell Attack via Email Phishing<br><br>


**### _Overview_** 

This project simulates a real-world cyberattack scenario in a controlled SOC (Security Operation Center) lab environment. It demonstrates both **offensive** and **defensive** security techniques, focusing on **Reverse shell Attacks** via **Email Phishing.** <br><br>


**### _Objectives_** 

- Simulate real-world attack scenarios
- Understand how attackers deliver payloads through phishing
-  practice post-exploitation techniques
- Set up a working SOC lab for future blue/red team practices <br><br>



**_### Lab Setup_**

- Kali Linux | Attacker machine
- Windows 10 | Victim machine
-  Metasploitable 2 | Vulnerable system
- VirtualBox | Virtualization environment
- MailHog | SMTP server simulation
- Gophish | Email phishing campaign tool
- Custom NAT Network: **meta-lab** (IPv4: 10.0.2.0/24 with DHCP) <br><br>


**### _Attack scenario: Reverse Shell via Email Phishing_**  

1. Payload creation using msfvenom
2. delivery of payload via phishing email using Gophish + MailHog (simulated SMTP server)
3. Execution on victim machine (windows 10) leads to reverse shell
4. Post-exploitation techniques:

- Persistence 
- File system interaction
- Obtaining system information <br><br>


**### _Tools and commands used_**

- Metasploit (msfvenom, multi/handler, Meterpreter)
- MailHog (Port: 1025 for SMTP, 8025 for web UI)
- Gophish (Phishing email template and delivery)
- ipconfig, sysinfo, getuid, netstat -ano for enumeration 
