[README.md](https://github.com/user-attachments/files/35312115/README.md)

# ⚡ AXIOMCYBER // Tactical Cyber & SDR Operations Center

[![Node.js](https://img.shields.io/badge/Node.js-v20%2B-026e00?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Electron](https://img.shields.io/badge/Electron-Desktop_App-47848F?style=for-the-badge&logo=electron&logoColor=white)](https://www.electronjs.org/)
[![Python](https://img.shields.io/badge/Python-3.10%2B_DSP-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org/)
[![HackRF](https://img.shields.io/badge/Hardware-HackRF_One-red?style=for-the-badge&logo=radio&logoColor=white)](https://greatscottgadgets.com/hackrf/one/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

> **AXIOMCYBER** is a cyberpunk-themed, full-stack Security Operations Center (SOC) dashboard, ethical hacking suite, and **Software Defined Radio (SDR) tactical console with native HackRF One integration**. Available as both a standalone desktop application (Electron) and a browser-based operations console.

---

```
  █████╗ ██╗  ██╗██╗ ██████╗ ███╗   ███╗ ██████╗██╗   ██╗██████╗ ███████╗██████╗ 
 ██╔══██╗╚██╗██╔╝██║██╔═══██╗████╗ ████║██╔════╝╚██╗ ██╔╝██╔══██╗██╔════╝██╔══██╗
 ███████║ ╚███╔╝ ██║██║   ██║██╔████╔██║██║      ╚████╔╝ ██████╔╝█████╗  ██████╔╝
 ██╔══██║ ██╔██╗ ██║██║   ██║██║╚██╔╝██║██║       ╚██╔╝  ██╔══██╗██╔══╝  ██╔══██╗
 ██║  ██║██╔╝ ██╗██║╚██████╔╝██║ ╚═╝ ██║╚██████╗   ██║   ██████╔╝███████╗██║  ██║
 ╚═╝  ╚═╝╚═╝  ╚═╝╚═╝ ╚═════╝ ╚═╝     ╚═╝ ╚═════╝   ╚═╝   ╚═════╝ ╚══════╝╚═╝  ╚═╝
              [ TACTICAL C2 // THREAT INTEL // RF OPERATIONS ]
```

---

## 🌟 Key Capabilities

### 1. 🌐 Interactive Global Cyber Threat Map
* **Dynamic Ballistic Attack Arcs**: Real-time animated trajectory curves on an HTML5 world map canvas plotting origins, targets, and threat signatures.
* **Impact Shockwaves**: Expanding ripple rings triggered upon payload arrival across critical sectors (Defense, Banking, Energy Grid, Healthcare).
* **Live WebSocket Telemetry**: Intercepted cyber attack stream displaying attacker IP, victim country, protocol, signature (Cobalt Strike C2, Citrix Bleed, Log4Shell, DDoS UDP, SQLi), and severity.

### 2. 🚨 Threat Intelligence & Hacker Group Syndicates
* **MITRE ATT&CK Group Profiles**: Deep-dive dossiers covering active state-sponsored units and ransomware cartels (LockBit 3.0, Scattered Spider, Lazarus Group, Volt Typhoon, Fancy Bear / APT28, Cl0p, BlackCat/ALPHV, Sandworm Team).
* **Live CISA KEV API Catalog**: Direct sync with the U.S. Cybersecurity and Infrastructure Security Agency's Known Exploited Vulnerabilities catalog with search and Ransomware-only filters.
* **Security Dispatches**: Aggregated real-time headlines and CVE disclosures from cybersecurity threat feeds.

### 3. 📡 Network Sentinel (Host Network Monitor)
* **Local Interface Interrogation**: Live adapters, IPv4/IPv6, MAC addresses, subnets, and CIDR masks.
* **ICMP Latency Oscilloscope**: Real-time ping latency graphing to root DNS targets (`8.8.8.8`) every 2 seconds.
* **Socket Inspector (`netstat -ano`)**: Real-time connection table with process IDs (PID), local/foreign endpoints, and connection states (`LISTENING`, `ESTABLISHED`, `TIME_WAIT`).
* **Subnet Radar (ARP Scan)**: Hardware MAC OUI vendor resolution (Apple, Intel, Samsung, TP-Link, Arcadyan router, etc.).

### 4. 🛠️ Built-in Ethical Hacker Arsenal
* **Async Multi-Threaded TCP Port Scanner**: High-speed socket probe with banner grabbing for common ports, web ports, database ports, or custom ranges.
* **DNS Reconnaissance**: Resolves `A`, `AAAA`, `MX`, `TXT` (SPF/DKIM/DMARC), `NS`, `CNAME`, `SOA`, and reverse `PTR` records.
* **IP & ASN Intelligence**: Instant BGP Autonomous System Number (`ASN`), ISP/Org, and geographic coordinate mapping.
* **HTTP Security Headers Auditor**: Audits `HSTS`, `CSP`, `X-Frame-Options`, `X-Content-Type-Options` with automated letter grades (**A+** to **F**).
* **SSL/TLS Certificate Inspector**: Direct TLS handshake inspecting validity period, days remaining, SANs, and cipher suite.
* **Subnet & CIDR Calculator**: Mask, wildcard, network, broadcast, and total usable IP ranges.
* **Cyber Decoder Suite**: Base64, Hex, URL, Binary, ROT13, and client-side SHA-256 hash generator.
* **Reverse Shell Payloads**: Authorized pentest command generators for Bash, Python, Netcat, PowerShell, and PHP.

---

## 📻 SDR & HACKRF ONE OPERATIONS

A complete Software Defined Radio operations deck tailored for **Great Scott Gadgets HackRF One**:

* **🔊 Live Audio Receiver & DSP Demodulator (`sdr_demod.py`)**:
  * Real-time 48 kHz 16-bit PCM streaming audio to your PC speakers.
  * **WFM**: FM broadcast radio (`88.0` - `108.0 MHz`) with 75 µs de-emphasis and polyphase decimation.
  * **NFM**: Walkie-talkies (FRS/GMRS/PMR446), NOAA Weather Radio (`162.400` - `162.550 MHz`), and 2m/70cm Ham repeaters.
  * **AM**: Aviation VHF Airband ATC (`118.0` - `137.0 MHz`) with envelope detection and DC removal.
  * Carrier squelch (`-90 dB` to `-20 dB`) and real-time audio waveform visualizer oscilloscope.
* **🎛️ Spectrum Analyzer & Cascading Waterfall**: Continuous tuning from `1 MHz` to `6000 MHz` (6 GHz) with adjustable LNA Gain (0-40 dB), VGA Gain (0-62 dB), and +14 dB RF amplifier toggle.
* **⚡ Live Hardware Cockpit**: Real-time HackRF USB bus detection, Board ID, Firmware Version, Part ID, and Serial Number.
* **🎯 1-Click Tactical Presets**: Quick-jump to FM, Airband, NOAA, 2m Ham, 70cm Ham, 433.92 MHz ISM, 315 MHz Car Keys, GSM Downlink, ADS-B 1090 MHz, GPS L1, Wi-Fi 2.4 GHz, and 5.8 GHz Drone FPV.
* **📡 Wideband Spectrum Sweeper (`hackrf_sweep`)**: Fast multi-frequency power level scanner to discover hidden transmitters and rogue beacons.
* **🎙️ Raw I/Q Capture & Replay (`hackrf_transfer`)**: Record raw I/Q samples to disk and transmit/replay signals for authorized RF security research.
* **🧮 Hardware Protocol Decoders**:
  * **ADS-B 1090 MHz Mode-S Decoder**: Extracts ICAO address, flight callsign (e.g. `KLM1023`), and altitude from raw hex frames.
  * **Sub-GHz Pulse Parser**: Decodes rolling code & EV1527 learning code remote controls.
* **🚀 Mayhem Mobile Integration**: 1-click launcher for **RocketGod's Mayhem Mobile** desktop PWA and direct web suite access.

---

## 💻 Interactive Hacker Command Terminal

Included terminal subsystem with command history (Up/Down arrows):

| Command | Action |
|---|---|
| `help` | Display interactive command manual |
| `listen [freq] [mode]` | Start live real-time SDR audio stream (e.g. `listen 98.5 WFM`) |
| `stopaudio` | Mute and release the active SDR audio stream |
| `tune <freq>` | Retune the SDR receiver (e.g. `tune 104.7` or `tune 433.92`) |
| `hackrf` | Interrogate connected HackRF hardware, firmware, and serial |
| `mayhem` | Launch RocketGod's Mayhem Mobile application |
| `sweep <start> <stop>` | Run wideband RF spectrum sweep (e.g. `sweep 88 108`) |
| `scan <host>` | Multi-threaded TCP port scan |
| `ping <host>` | ICMP round-trip latency test |
| `dns <domain>` | Enumerate DNS records (`A`, `MX`, `TXT`, `NS`) |
| `recon <ip>` | Query BGP ASN, ISP, and GeoIP registry data |
| `cisa <keyword>` | Query active exploited CVEs from CISA KEV catalog |
| `actors` | List nation-state & ransomware syndicate profiles |
| `matrix` | Toggle digital rain screen overlay |
| `theme <name>` | Switch HUD theme (`cyber`, `matrix`, `amber`, `red`) |
| `defcon <1-5>` | Override threat alert DEFCON posture |
| `audio` | Toggle procedural Web Audio sound FX |
| `clear` | Flush terminal log buffer |

---

## 🚀 Installation & Quick Start

### Prerequisites
* [Node.js](https://nodejs.org/) v18+ (tested on v20 / v26)
* [Python](https://python.org/) 3.9+ with `numpy` and `scipy` (`pip install numpy scipy`)
* Optional (for SDR features): [HackRF Tools](https://github.com/greatscottgadgets/hackrf) (`hackrf_info`, `hackrf_transfer`, `hackrf_sweep`)

### Quick Setup

```bash
# 1. Clone repository
git clone https://github.com/your-username/AxiomCyber.git
cd AxiomCyber

# 2. Install dependencies
npm install

# 3. Launch as Standalone Desktop App
npm run app
```

*Or to run in standard browser mode:*
```bash
npm start
# Open http://localhost:3333 in your browser
```

---

## 🎨 Themes & Audio Customization
* **Themes**: Cyberpunk Neon (Cyan/Magenta), Matrix Emerald, Amber CRT Terminal, and Crimson Breach.
* **Synthesized Web Audio FX**: Procedural sci-fi clicks, alarms, and scan sweeps generated via Web Audio API.

---

## ⚠️ Legal & Ethical Disclaimer
AXIOMCYBER is developed strictly for authorized cybersecurity testing, educational research, network administration, and licensed amateur radio experimentation. Transmitting radio frequencies without appropriate licensing or authorization is strictly prohibited by law (e.g., FCC regulations). Use responsibly.
