<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png">
    <img src="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png" alt="WiFi QR Code Generator" width="120">
  </picture>
</p>

<h1 align="center">WiFi QR Code Generator</h1>

<p align="center">
  <b>Turn your WiFi credentials into a scannable QR card — instantly, offline, no backend.</b>
</p>

<p align="center">
  <a href="https://sampark-lodge.github.io/wifi-qr-generator/">
    <img src="https://img.shields.io/badge/🌐_Live_Demo-00d4aa?style=for-the-badge&logo=githubpages&logoColor=white" alt="Live Demo">
  </a>
  <a href="https://github.com/Sampark-Lodge/wifi-qr-generator">
    <img src="https://img.shields.io/github/stars/Sampark-Lodge/wifi-qr-generator?style=for-the-badge&logo=github&color=00d4aa" alt="Stars">
  </a>
  <a href="https://github.com/Sampark-Lodge/wifi-qr-generator/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-00d4aa?style=for-the-badge" alt="License">
  </a>
  <br>
  <img src="https://img.shields.io/badge/uses-no%20cookies-00d4aa?style=flat-square" alt="No Cookies">
  <img src="https://img.shields.io/badge/privacy-100%25%20offline-00d4aa?style=flat-square" alt="100% Offline">
  <img src="https://img.shields.io/badge/size-4.2%20KB%20gzipped-00d4aa?style=flat-square" alt="Size">
  <img src="https://img.shields.io/badge/dependencies-1%20(qrcode.js)-00d4aa?style=flat-square" alt="Dependencies">
</p>

<br>

---

## 📸 Preview

<p align="center">
  <img src="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png" alt="App Screenshot" width="700">
</p>

<br>

## ✨ Features at a Glance

| | Feature | 
|---|---|
| ⚡ | **Live QR generation** — QR updates as you type, zero latency |
| 🔒 | **100% offline** — nothing leaves your device. No backend. No tracking |
| 🖨️ | **Printable card** — one-tap print with a clean, card-ready layout |
| 📥 | **Download as PNG** — export the QR code for signs, stickers, menus |
| 👁️ | **Password visibility toggle** — show/hide with a click |
| 🎨 | **Dark themed** — easy on the eyes, modern teal-accent design |
| 📱 | **Fully responsive** — works on phone, tablet, and desktop |
| 📋 | **WPA/WPA2, WEP, or Open** — supports all security types |

<br>

## 🎯 How It Works

```
Enter SSID  →  Set Password  →  Choose Security  →  Scan & Connect
     │              │                 │                    │
     └──────────────┴─────────────────┘                    │
                      │                                    │
              QR regenerates                          Guest scans
              automatically                          QR to connect
```

<p align="center">
  <em>QR encodes the standard <code>WIFI:T:WPA;S:MyNetwork;P:MyPassword;;</code> format — works with every modern phone camera.</em>
</p>

<br>

## 🖼️ Visual Walkthrough

### 1. Form Input
> Dark card with Outfit typography, teal focus rings, custom select dropdown arrows.

<img src="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png" alt="Form input" width="400">

### 2. Live QR Code
> White-backed QR (for scanner contrast) renders instantly as you fill fields.

<img src="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png" alt="QR display" width="400">

### 3. Printable Network Card
> Bold network name (32px, 700 weight), monospace password (JetBrains Mono, teal), scan label.

<img src="https://sampark-lodge.github.io/wifi-qr-generator/wifi-qr-preview.png" alt="Print card" width="400">

### 4. Print Preview
> `@media print` hides everything except the card — clean print, no wasted ink.

<br>

## 🚀 Usage

```bash
# Clone
git clone https://github.com/Sampark-Lodge/wifi-qr-generator.git

# Open — that's it (it's a single HTML file)
open index.html
```

Or just use it directly at **https://sampark-lodge.github.io/wifi-qr-generator/** — no install needed.

<br>

## 🎨 Visual Design System

| Token | Value | Preview |
|---|---|---|
| `--bg` | `#0f0f0f` | ![near black](https://via.placeholder.com/16/0f0f0f/000000?text=+) Near black |
| `--card-bg` | `#1a1a1a` | ![dark gray](https://via.placeholder.com/16/1a1a1a/000000?text=+) Dark gray |
| `--input-bg` | `#2a2a2a` | ![input gray](https://via.placeholder.com/16/2a2a2a/000000?text=+) Input bg |
| `--accent` | `#00d4aa` | ![teal](https://via.placeholder.com/16/00d4aa/000000?text=+) Teal/mint |
| `--text` | `#ffffff` | ![white](https://via.placeholder.com/16/ffffff/000000?text=+) White |
| `--text-muted` | `#888888` | ![muted](https://via.placeholder.com/16/888888/000000?text=+) Muted gray |
| `--border` | `#333333` | ![border](https://via.placeholder.com/16/333333/000000?text=+) Subtle border |

| Typography | Usage |
|---|---|
| **Outfit** (sans-serif) | Headings, labels, inputs — modern geometric |
| **JetBrains Mono** (monospace) | Password display on the printable card |

<br>

## 🧱 Tech Stack

```
┌─────────────────────────────────────────────┐
│              index.html (4.2 KB gz)           │
│  ┌──────────┐  ┌──────────┐  ┌───────────┐  │
│  │  HTML5   │  │  CSS3    │  │  Vanilla  │  │
│  │  Semanti │  │  Flexbox │  │   JS      │  │
│  │  c       │  │  Custom  │  │  (no      │  │
│  │  struct  │  │  Props   │  │  framework│  │
│  │  ure     │  │  :root   │  │  )        │  │
│  └──────────┘  └──────────┘  └───────────┘  │
│                                              │
│  External: qrcodejs (CDN) — QR generation    │
│  Hosting: GitHub Pages                       │
└─────────────────────────────────────────────┘
```

- **Zero build tools** — no webpack, no npm install, no config
- **Zero server** — everything runs in the browser
- **Zero tracking** — no analytics, no cookies, no telemetry
- **One dependency** — `qrcodejs` from CDN

<br>

## 📐 Responsive Breakpoints

| Viewport | Layout |
|---|---|
| **< 480px** (mobile) | Full-width card, reduced padding |
| **480px+** (tablet) | Centered card, max-width 480px |
| **768px+** (desktop) | Same centered layout, comfortable spacing |

<br>

## 📄 File Structure

```
wifi-qr-generator/
├── index.html          ← The entire app (HTML + CSS + JS)
├── robots.txt          ← Search engine crawl rules
├── sitemap.xml         ← SEO sitemap
├── SPEC.md             ← Design & functional spec
├── ssl-cert-checker/   ← (sibling tool)
├── ui-ux-pro-max-skill/
└── README.md           ← You are here
```

<br>

## 🧪 QR Format Reference

| Security | Generated String |
|---|---|
| WPA/WPA2 | `WIFI:T:WPA;S:MyNetwork;P:secret123;;` |
| WEP | `WIFI:T:WEP;S:MyNetwork;P:secret123;;` |
| None (Open) | `WIFI:T:nopass;S:MyNetwork;P:;;` |

<br>

## 🔐 Privacy

> **Your password never leaves this page.**

No data is transmitted, stored, or logged. The QR code is generated entirely in your browser. The page works fully offline after the first load.

<p align="center">
  <img src="https://img.shields.io/badge/✅_NO_server_requests-00d4aa?style=flat-square" alt="No server">
  <img src="https://img.shields.io/badge/✅_NO_cookies-00d4aa?style=flat-square" alt="No cookies">
  <img src="https://img.shields.io/badge/✅_NO_analytics-00d4aa?style=flat-square" alt="No analytics">
  <img src="https://img.shields.io/badge/✅_NO_telemetry-00d4aa?style=flat-square" alt="No telemetry">
</p>

<br>

## 📬 Use Cases

- 🏨 **Hotels & lodges** — print QR cards for guest room WiFi
- ☕ **Cafés & restaurants** — laminate QR tent cards for tables
- 🏢 **Offices** — stick QR on meeting room walls
- 🏠 **Home** — share guest network without spelling passwords
- 🎪 **Events** — quick WiFi access for attendees

<br>

---

<p align="center">
  <sub>Built with ❤️ for Sampark Lodge · Made in India 🇮🇳</sub>
  <br>
  <sub>
    <a href="https://sampark-lodge.github.io/wifi-qr-generator/">Launch App</a> ·
    <a href="https://github.com/Sampark-Lodge/wifi-qr-generator/issues">Report Issue</a>
  </sub>
</p>
