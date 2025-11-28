---
title: XIAO NRF 52840
---

### XIAO nRF52840
Intro:
The XIAO nRF52840 is a tiny, ultra‑low‑power development board from Seeed Studio that’s fully compatible with Meshtastic. Despite its small size, it packs Bluetooth 5.0, LoRa support (via external modules), and flexible power options, making it ideal for discreet or wearable mesh nodes.

Key Features:
- MCU: Nordic nRF52840 ARM Cortex‑M4F (Bluetooth 5.0, BLE, NFC)
- Memory: 1 MB Flash, 256 KB RAM
- Connectivity:
- Native Bluetooth 5.0
- LoRa via external SX1262/SX1276 modules
- Power Options:
- USB‑C interface
- Li‑Po battery connector
- Ultra‑low‑power sleep modes for extended runtime
- Form Factor:
- Extremely compact (21 × 17.5 mm)
- 11 GPIO pins for expansion
- Programming: UF2 bootloader support for drag‑and‑drop firmware flashing

Considerations:
- Requires external LoRa module for full Meshtastic functionality (not built‑in like Heltec boards)
- Very small size limits antenna options and onboard features (no display)
- Best suited for wearable, discreet, or embedded nodes where space and power efficiency matter
- Less beginner‑friendly compared to T‑Beam or Heltec V3 — better for advanced operators comfortable with modular builds
- Ideal for custom enclosures, sensor integration, or stealth deployments in Iowa Mesh




{{< imgproc "xiao-nrf52840-sense-plus.jpg" Resize "600x" >}}