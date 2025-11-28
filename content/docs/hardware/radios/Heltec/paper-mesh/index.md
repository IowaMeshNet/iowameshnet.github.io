---
title: Paper Mesh
---

### Heltec Wireless Paper (Paper Mesh)
Intro:
The Wireless Paper is Heltec’s e‑ink variant of their LoRa boards, built for Meshtastic. It combines the ESP32 MCU with the SX1262 LoRa transceiver and a 2.13″ e‑ink screen, making it ideal for low‑power, always‑visible status displays in a mesh network.

Key Features:
- MCU: ESP32‑S3FN8 with Wi‑Fi and Bluetooth support
- LoRa Transceiver: Semtech SX1262
- Frequency Options: 433 MHz, 470–510 MHz, 863–870 MHz, 902–928 MHz
- Display: 2.13″ e‑ink screen (black/white, ultra‑low power)
- Connectors: USB‑C for power/programming, U.FL/IPEX antenna connector
- Form Factor: Slim board with acrylic protection option
- Power: SH1.25 battery connector for external Li‑Po packs

Considerations:
- Screen support varies by firmware version — some revisions (e.g., V1.1.1) had issues with e‑ink compatibility.
- No case included — operators often need to 3D‑print or adapt enclosures.
- Best for fixed or semi‑portable nodes where low‑power display is useful (status, packet counts, node ID).
- Not as rugged as Station‑class devices — better suited for hobbyist or indoor deployments.
- Affordable option (~$17–20 on AliExpress) compared to OLED boards.






{{< imgproc "Paper-Meshtastic.jpg" Resize "300x" >}}