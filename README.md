# kali-gui
Run Kali Linux GUI in Docker with noVNC (Browser Access) — works on AMD64 &amp; ARM64

# Kali Linux GUI in Docker (with noVNC Browser Access)

Run Kali Linux with XFCE desktop environment inside Docker and access it directly from your browser using noVNC.  
Supports **AMD64** and **ARM64** (including Apple Silicon).

---

## ✨ Features
- Full Kali Linux XFCE desktop in your browser
- Accessible over **localhost** or LAN
- Built-in **Virtual Keyboard** for touchscreen devices
- Works on **AMD64** (Intel/AMD PCs) and **ARM64** (Mac M1/M2, Raspberry Pi)
- noVNC auto-adjustable for various screen sizes

---

## 📦 Build Instructions

### 1. Clone the repository
```bash
git clone https://github.com/iKryptonian/kali-gui.git
cd kali-gui-novnc
2. Build the image
For AMD64 (Intel/AMD PCs):
docker buildx build --platform linux/amd64 -t kaligui:latest .
For ARM64 (Apple M1/M2, Raspberry Pi):
docker buildx build --platform linux/arm64 -t kaligui:latest .
3. Run the container
docker run -it -p 6080:6080 kaligui
