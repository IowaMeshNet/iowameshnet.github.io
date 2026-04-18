---
date: 2025-06-26
title: Meshtastic v2.7 Technical Preview
author: Chad Porter ([EMB3D](emb3dthreat@proton.me))
---

## Meshtastic v2.7 Technical Preview: BaseUI & Key Verification
Meshtastic recently announced firmware v2.7 Technical Preview, a major update that brings a fresh look, new features, and a big step forward in secure communication for the IowaMesh community.

### 1. BaseUI: A Fresh Interface
After four years, the default Meshtastic interface finally gets a name and full redesign. BaseUI is more intuitive, more capable, and optimized for a wide range of devices, from OLED screens to basic TFTs.

**Base UI New Features:**
1. Set region & timezone directly on-device
1. Digital 12/24-hour clock
1. Auto-hiding menu bar with action menus for Home, Messages, GPS, LoRa, & System

### 2. Key Verification: A New Layer of Trust
One of the most exciting additions in 2.7 for me is the Key Verification feature. This allows users to verify secure communication between devices using a six-digit code.

**How It Works:**
1. Select a node and tap "Initiate Verification"
1. A six-digit code gets generated, securely send the code to the recieving device
1. Both devices should receive a confirmation code, proving they’re securely communicating

This is a big step toward improving the security of Meshtastic networks. Future updates may even allow re-keying between devices.

**Note:** While Key Verification is available in v2.7 Technical Preview now, full client support has not been released yet.