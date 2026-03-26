# Self-Hosted Blog on Ubuntu Server

**Hardware:** MacBook Pro M4  

A complete **on-demand self-hosted blog** running inside a Ubuntu Server virtual machine. The blog only runs when I turn on the VM — perfect for a private portfolio.

### Project Goal
Build my own private hosting server from scratch to host a personal cybersecurity blog/portfolio.
<img width="1504" height="966" alt="Screenshot 2026-03-26 at 8 30 46 PM" src="https://github.com/user-attachments/assets/dda7c3e1-788f-4d25-9ca9-7b5d8aeb170c" />


## Step-by-Step Tutorial

### 1. Create the Ubuntu Server VM in UTM
- Download **Ubuntu Server 24.04.4 LTS ARM64** ISO
- Open UTM -> Click "Create a New Virtual Machine" -> "Virtualize" -> "Linux" -> Hardware -> Storage
- Created new VM in UTM:
  - 2 CPU cores
  - 2 GB RAM
  - 20 GB storage
- Installed Ubuntu Server with OpenSSH enabled

<img width="1364" height="891" alt="Screenshot 2026-03-21 at 11 22 48 AM" src="https://github.com/user-attachments/assets/832f55eb-abe3-4c50-8ca2-4f27abf32c10" />
<img width="539" height="41" alt="Screenshot 2026-03-21 at 11 45 43 AM" src="https://github.com/user-attachments/assets/2d69b65e-2ff2-4d32-86e8-29590c1a2cdb" />

### 2. Initial Server Setup
- Updated system: "sudo apt update && sudo apt upgrade -y"
- Installed essential packages: "sudo apt install nginx git curl unzip snapd -y"
- Installed Hugo: "sudo snap install hugo"

### 3. Set Up the Hugo Blog
- Created blog directory: "mkdir ~/blog && cd ~/blog"
- Initialized Hugo site
- Added **PaperMod** theme
- Created "hugo.toml" configuration

### 4. Configure Nginx Web Server
- Moved built site to "/var/www/html"
- Created clean Nginx configuration
- Set proper permissions
- Restarted Nginx service

### 5. Make It Accessible
- Blog is available locally
- Can be exposed publicly using ngrok when needed (on-demand)

## Why This Project is Valuable for a Cybersecurity Analyst
Even though this is a blog server, the skills directly translate to real security operations:
- Managing Linux systems
- Configuring services securely
- Troubleshooting configuration and permission issues
- Building and maintaining infrastructure
- Creating technical documentation

## Tech Stack
- **Virtualization**: UTM 
- **Operating System**: Ubuntu Server 24.04 LTS
- **Web Server**: Nginx
- **Site Generator**: Hugo + PaperMod theme
- **Access**: SSH

## Screenshots
<img width="908" height="662" alt="Screenshot 2026-03-21 at 11 20 45 AM" src="https://github.com/user-attachments/assets/a9a98bbf-ff48-4002-bb0e-747e3e2190cd" />
<img width="907" height="655" alt="Screenshot 2026-03-21 at 11 20 53 AM" src="https://github.com/user-attachments/assets/ae7fcc61-eea5-4035-9b38-b1495840d4d9" />
<img width="912" height="652" alt="Screenshot 2026-03-21 at 11 21 03 AM" src="https://github.com/user-attachments/assets/671e949d-cddc-4f8b-9a74-476823313916" />
<img width="909" height="657" alt="Screenshot 2026-03-21 at 11 22 13 AM" src="https://github.com/user-attachments/assets/0e98dc20-e8fb-4a93-a685-c8c1795376f3" />
<img width="906" height="655" alt="Screenshot 2026-03-21 at 11 46 12 AM" src="https://github.com/user-attachments/assets/9003a68e-d6f5-46fd-a583-9ab07360248c" />
<img width="1280" height="839" alt="Screenshot 2026-03-21 at 11 46 45 AM" src="https://github.com/user-attachments/assets/801a55d6-08ca-4a32-8306-56184f89172f" />
<img width="1289" height="842" alt="Screenshot 2026-03-21 at 11 47 00 AM" src="https://github.com/user-attachments/assets/ad660420-bdf1-4a0a-89d7-5fc5fd58c38b" />
<img width="1280" height="840" alt="Screenshot 2026-03-21 at 11 51 24 AM" src="https://github.com/user-attachments/assets/1a7067d3-f680-45b5-8553-b8fe4490fa00" />
<img width="1278" height="837" alt="Screenshot 2026-03-21 at 11 58 29 AM" src="https://github.com/user-attachments/assets/fa1e328d-f6bc-4692-94b6-b7e7e12a8dae" />
<img width="1287" height="842" alt="Screenshot 2026-03-21 at 11 59 38 AM" src="https://github.com/user-attachments/assets/ad2980e2-8512-4bfb-95b1-8bd9f1d82070" />
<img width="1275" height="842" alt="Screenshot 2026-03-21 at 11 59 51 AM" src="https://github.com/user-attachments/assets/c759359c-65df-4af0-98cd-5a8e788d37b3" />
<img width="1282" height="842" alt="Screenshot 2026-03-21 at 12 01 19 PM" src="https://github.com/user-attachments/assets/263fd03d-5b31-4d8b-a247-49b4fc04b8ff" />
<img width="1282" height="838" alt="Screenshot 2026-03-21 at 12 02 51 PM" src="https://github.com/user-attachments/assets/2b3e1bf3-354c-4c17-b629-b2a8f6480f68" />
<img width="1270" height="832" alt="Screenshot 2026-03-21 at 12 07 52 PM" src="https://github.com/user-attachments/assets/da335cb5-6ee4-4a78-9888-8bc10497a993" />
<img width="900" height="998" alt="Screenshot 2026-03-26 at 8 32 57 PM" src="https://github.com/user-attachments/assets/5d8e1b34-78fc-45c4-9fde-7dd1af9500da" />

## Usefull for
- Private Hosting
- Personal Blog


This repo show how I build private a hosting server and blog.

