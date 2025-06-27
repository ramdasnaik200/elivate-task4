# 🔒 Firewall Configuration Practice

This project contains the steps I followed to practice basic firewall configuration on both **Windows** and **Linux** systems.

---

## ✅ What I Did

1. Opened the firewall tool:
   - Used **PowerShell (Admin)** on Windows
   - Used **UFW (Uncomplicated Firewall)** on Linux

2. Listed current firewall rules to understand the default configuration.

3. Created a rule to **block inbound traffic on port 23** (Telnet) to prevent unsecured access.

4. Tested the rule by trying to connect to port 23 from another machine using Telnet.

5. On Linux, I added a rule to **allow SSH (port 22)** to ensure remote access is not blocked.

6. Removed the Telnet block rule to **restore the original firewall state**.

7. Verified each step using `telnet`, `netstat`, and firewall rule listing commands.

---

## 🔧 Tools and Commands Used

### Windows (PowerShell)
- `Get-NetFirewallRule`
- `New-NetFirewallRule`
- `Remove-NetFirewallRule`

### Linux (UFW)
- `sudo ufw status`
- `sudo ufw deny 23/tcp`
- `sudo ufw allow 22/tcp`
- `sudo ufw delete deny 23/tcp`

---

## 📚 Summary

This task helped me understand how firewalls control network traffic by using rules to **allow or block specific ports**. It also showed how to test firewall configurations using tools like **Telnet** and commands like **netstat**.

---
