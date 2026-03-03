# Network Attack Detection & Reporting (SSH Honeypot Lab)

## 📌 Overview
This project focuses on detecting and analyzing SSH-based network attacks using a honeypot environment. I deployed Cowrie Honeypot on Ubuntu to simulate an SSH server and monitored attacker activity using Wireshark.

The objective was to understand how attackers perform reconnaissance and brute-force attempts, and how defenders detect such activity at the network level.

---

## 🛠 Tools & Technologies
- Nmap (Reconnaissance & Port Scanning)
- Wireshark (Packet Capture & Traffic Analysis)
- Kali Linux (Attacker Machine)
- Ubuntu Server (Target Machine)
- Cowrie Honeypot (SSH Honeypot)

---

## 🔬 Lab Architecture
- Attacker: Kali Linux
- Target: Ubuntu running Cowrie Honeypot
- Monitoring Tool: Wireshark
- Network: Internal Virtual Lab (VMware)

---

## 🧪 Attack Simulation
1. Performed Nmap scans to identify open ports.
2. Discovered open SSH port.
3. Simulated SSH login attempts against Cowrie.
4. Captured and analyzed SSH traffic using Wireshark.
5. Reviewed Cowrie logs for attack details.

---

## 📊 Detection & Analysis
- Identified TCP handshake for SSH sessions
- Observed repeated login attempts (Brute Force behavior)
- Analyzed source IP addresses
- Correlated Wireshark captures with Cowrie logs
- Documented timestamps and attack patterns

---

## 📝 Reporting
Each attack was documented with:
- Source IP
- Destination IP
- Port number
- Attack type (SSH brute force / reconnaissance)
- Packet evidence
- Honeypot log evidence
- Mitigation recommendations

---

## 🛡 Skills Demonstrated
- Network traffic analysis
- SSH protocol inspection
- Honeypot deployment
- Threat detection
- Log correlation
- Incident reporting (SOC workflow)

---

## 🚀 Future Improvements
- Integrate with Wazuh SIEM
- Create automated alerting system
- Deploy multiple honeypots
- Implement firewall blocking rules
