
---

## 1️⃣ What You’ll Build

✅ A secure Linux VM with UFW firewall.  
✅ Allow only **SSH (22), HTTP (80), HTTPS (443)**.  
✅ Block everything else by default.  
✅ Optional **Python Auto-Blocker** to dynamically ban brute-force SSH attackers.  

**High-level diagram**:  

Laptop → Internet → Linux VM (UFW) → Allowed Ports → Web App

---

## 2️⃣ Prerequisites

- Ubuntu 22.04/24.04 VM (VirtualBox/VMware/WSL) or Cloud VM (AWS/GCP).  
- User with sudo privileges.  
- Internet connection.  

---

## 3️⃣ Install & Enable UFW

Check status and install if missing:
```bash
sudo ufw status
sudo apt install ufw -y
