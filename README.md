# kali-gui

**Run Kali Linux GUI in Docker with noVNC (Browser Access) — Works on AMD64 & ARM64**  

Easily run Kali Linux with the XFCE desktop environment inside Docker and access it directly from your browser using **noVNC**.  
Supports both **AMD64** and **ARM64** (including Apple Silicon Macs).

---

## ✨ Features

- 🖥 **Full Kali Linux XFCE Desktop** in your browser  
- 🌐 **Accessible over localhost or LAN**  
- ⌨ **Built-in Virtual Keyboard** for touchscreen devices  
- ⚡ Works on **AMD64** (Intel/AMD PCs) and **ARM64** (Mac M1/M2, Raspberry Pi)  
- 📱 **noVNC auto-adjustable** for various screen sizes  

---

## 📦 Build Instructions

### 1️⃣ Clone the repository

git clone https://github.com/iKryptonian/docker-kali-gui.git
cd kali-gui

---

### 2️⃣ Build the Docker image

For AMD64 (Intel/AMD PCs):  
docker buildx build --platform linux/amd64 -t kaligui:latest .

For ARM64 (Apple M1/M2, Raspberry Pi):  
docker buildx build --platform linux/arm64 -t kaligui:latest .

---

### 3️⃣ Run the container

docker run -it -p 6080:6080 kaligui

---

## 🚀 Access Kali GUI

Once running, open your browser and go to:  
👉 **http://localhost:6080**  

---


