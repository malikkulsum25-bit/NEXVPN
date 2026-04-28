# ⬡ NEXVPN — Advanced Privacy System

A full-stack VPN dashboard with real network measurements, threat intelligence, and privacy tools.

## 🚀 Quick Start

### 1. Backend
```bash
cd backend
npm install
node server.js
# Runs on http://localhost:3001
```

### 2. Frontend
```bash
cd frontend
npm install
npm start
# Runs on http://localhost:3000
```

## ✨ Unique Features

### 🔒 Privacy Score (NEW)
- Dynamic 0–100 score calculated from your active security settings
- Animated canvas ring visualization
- Live checklist showing exactly what's protecting you and what's missing
- Quick action buttons to fix gaps

### ☠️ Threat Intelligence (NEW)
- **Live event feed** — real-time display of blocked trackers, suspicious IPs, DNS blocks
- **IP threat scan** — queries your public IP against threat intelligence databases
- **Domain reputation scanner** — analyze any domain for malicious patterns and tracking

### 🔍 WebRTC & DNS Leak Detector (NEW)
- **Real WebRTC leak test** — uses your browser's WebRTC API to detect IP leaks through ICE candidates
- **DNS leak test** — checks if your DNS queries are visible outside the VPN tunnel
- Actionable remediation advice for each finding

### 🗺️ GeoSpoof Visualizer (NEW)
- **Animated world map** with real-time tunnel visualization
- Shows your real location (red) vs masked exit node (green)
- Animated dashed line showing the encrypted tunnel path
- Displays real IP data from geolocation APIs

### 📊 Privacy Score Dashboard
- Real-time score updates as you change settings
- Integrated quick-action panel

## Real Network Features
- **Real TCP latency** measurements to VPN servers
- **Actual download speed** test via Cloudflare CDN (2MB sample)
- **Real public IP** detection with multi-API geolocation fallback
- **Real DNS leak** testing against live domains
- **WebSocket-based** encrypted peer-to-peer chat (AES-256)
- **RSA-2048 key exchange** for encryption handshakes

## Architecture
- **Frontend**: React.js with JetBrains Mono + Syne fonts, dark cyberpunk theme
- **Backend**: Node.js + Express + Socket.IO
- **Auth**: JWT tokens + bcrypt password hashing
- **Encryption**: RSA-2048 key pairs + AES-256-CBC per session
