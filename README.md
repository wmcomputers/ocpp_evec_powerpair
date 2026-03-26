# OCPP (EVEC PowerPair Patch)

⚠️ **This is a patched fork of the original project and is not the official repository.**

---

## 🔧 About This Fork

This repository contains a **patched version** of the Home Assistant OCPP integration to support the **EVEC PowerPair dual connector charger**.

The EVEC PowerPair charger:
- Uses OCPP 1.6
- Exposes multiple connectors in runtime traffic
- Does **not correctly respond** to `NumberOfConnectors` configuration requests

Because of this, the original integration detects only a single connector.

### ✅ What this patch does

- Forces Home Assistant to correctly initialise **2 connectors**
- Ensures both connectors are:
  - Discovered
  - Created as entities
  - Fully usable in Home Assistant

---

## 🙌 Credit to Original Project

All credit for this integration goes to the original author:

👉 https://github.com/lbbrhzn/ocpp

This fork is **only a small compatibility patch** and builds entirely on their work.

If you are using a standard OCPP charger, you should use the original project instead.

---

## 📦 Original Project Description

This is a Home Assistant integration for Electric Vehicle chargers that support:

- OCPP 1.6j  
- OCPP 2.0.1  
- OCPP 2.1 (experimental)

Based on the Python OCPP package:  
👉 https://github.com/mobilityhouse/ocpp

Documentation:  
👉 https://home-assistant-ocpp.readthedocs.io

---

## ⚠️ When Should You Use This Fork?

Use this fork **only if you have an EVEC PowerPair charger** and experience:

- Only 1 connector appearing in Home Assistant
- Missing entities for the second connector

Otherwise, use the official integration.

---

## 💡 Tip

If you like the original project, consider supporting the author:

https://www.buymeacoffee.com/lbbrhzn

---

## 📌 Disclaimer

This fork is not affiliated with or endorsed by the original author.  
It exists purely to address a device-specific compatibility issue.
