# Hello World Full Stack App (Django + React)

This is a simple full-stack application demonstrating integration between a Django REST API backend and a React micro frontend (MFE), running together using Docker Compose.

---

## 🛠️ Tech Stack

- **Backend**: Django, Django REST Framework
- **Frontend**: React (via Create React App)
- **Containerization**: Docker, Docker Compose
- **CORS**: Enabled for cross-origin requests from React to Django

---

## 🚀 Quick Start

### 🔁 1. Clone the Repository

```bash
git clone https://github.com/SkillUpTech/demo-sample.git
cd demo-sample
docker compose up --build
```

This will:

Start the Django backend on http://localhost:8000

Start the React frontend on http://localhost:8080

Open your browser and go to:

http://localhost:8080

You should see:

Hello, World!



# Docker Installation Guide

This document provides step-by-step instructions to install Docker on **Windows** and **Ubuntu**.

---

## Windows (10/11 Pro, Enterprise, or Education)

### System Requirements
- 64-bit processor with SLAT support
- Virtualization enabled in BIOS
- Windows 10/11 Pro, Enterprise, or Education (Home requires WSL 2)

### Installation Steps

1. Download Docker Desktop installer from [Docker official site](https://www.docker.com/products/docker-desktop/)
2. Run the installer and follow the setup wizard
3. If using Windows Home, ensure WSL 2 is installed and enabled (Docker Desktop installer will help)
4. Restart your computer if prompted
5. Open PowerShell or Command Prompt and verify installation:
   ```powershell
   docker --version
   docker run hello-world

## Ubuntu

```
sudo apt-get update
sudo apt-get install -y ca-certificates curl gnupg

sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg

echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] \
  https://download.docker.com/linux/ubuntu \
  $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update
sudo apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

sudo usermod -aG docker $USER
```
Reboot the system

