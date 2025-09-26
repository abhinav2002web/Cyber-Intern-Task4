# Cyber-Intern-Task4

# 🔐 Task 4: Setup and Use a Firewall on Linux (UFW)

This project demonstrates how to configure and test basic firewall rules on a Linux system using **UFW (Uncomplicated Firewall)**.

---

## 🎯 Objective
Configure and test basic firewall rules to **allow or block traffic** using the terminal in a Kali Linux environment.

---

## 🧰 Tools Used
- 🐧 **Operating System**: Kali Linux
- 🔥 **Firewall Tool**: UFW (Uncomplicated Firewall)
- 🖥️ **Terminal-based Commands**

---

## 📝 Steps Performed

### ✅ 1. Enable the Firewall
```bash
sudo ufw enable
```

### ✅ 2. Check Current Rules
```bash
sudo ufw status numbered
```

### ✅ 3. Block Port 23 (Telnet)
```bash
sudo ufw deny 23
```

### ✅ 4. Test Blocked Port
```bash
telnet localhost 23
```
Expected output: _Connection refused_

### ✅ 5. Allow Port 22 (SSH)
```bash
sudo ufw allow 22
```

### ✅ 6. Remove Block Rule on Port 23
```bash
sudo ufw delete deny 23
```

---

## 🖼️ Screenshot

> The image `task4.jpg` shows all the above commands and their outputs on a Kali Linux terminal.

---

## 🧠 How UFW Filters Traffic

UFW (Uncomplicated Firewall) is a frontend for iptables. It allows you to:
- Easily allow or deny traffic on specific ports
- Configure inbound/outbound rules
- Protect your system by blocking unnecessary services

UFW enforces these rules at the kernel level, filtering traffic **before it reaches your applications**.

---

## ✅ Outcome

You will gain basic firewall configuration skills, including:
- Enabling UFW
- Blocking and allowing ports
- Testing firewall behavior
- Cleaning up firewall rules
