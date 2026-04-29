
# 🚀 Azure Linux VM + Nginx Deployment

## 📌 Objective
Deploy a Linux Virtual Machine in Azure and host a web server using Nginx.

---

## 🛠️ Technologies Used
- Microsoft Azure
- Linux (Ubuntu 22.04)
- Nginx
- SSH

---

## ⚙️ Steps Performed

### 1. Created Azure VM
- Ubuntu 22.04
- Size: B1s
- SSH authentication enabled

### 2. Connected via SSH
```bash
ssh -i vm-key.pem azureuser@<public-ip>
**
3.Installed Nginx

sudo apt update
sudo apt install nginx -y

4.Started Service
sudo systemctl start nginx

5.Configured Networking

Opened port 80 in Azure NSG

6.Verified Deployment

Access via browser using public ip
Successfully loaded nginx deafult page
