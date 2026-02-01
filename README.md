# TunnelFireSurrogateModelling
# Tunnel Fire Temperature Field Dataset (FDS-based)

This repository provides the metadata, documentation, and access links for the tunnel fire temperature-field dataset used in our paper:
**"[Paper Title]"** (Year).

> **Note:** Due to the large size of the raw data, the dataset files are hosted on Baidu Netdisk. This GitHub repository contains documentation, metadata, checksums, and minimal loading examples.

---

## Dataset Overview
- Simulator: Fire Dynamics Simulator (FDS) v6.7.x
- Geometry: Tunnel length [100 m / 120 m / ...], height [7.2 m], width [6 m] (2D slice via 1 cell in transverse direction)
- Ambient: 20 °C, 101.325 kPa
- Outputs: temperature **T**, longitudinal velocity **U**, vertical velocity **W**
- Sampling: Δt = 1 s, total frames = 601 (0–600 s)
- Grid: H × W = 37 × 501 (z × x)  (adjust if yours differs)
- Global conditions: PHRR (MW), fire location xf (m), ventilation velocity v_vent (m/s), tunnel slope (%)

---

## Download
### Baidu Netdisk
- Link: [Baidu Netdisk Download]([PASTE_LINK_HERE])
- Extraction code (提取码): **[XXXX]**

**Recommended:** Verify file integrity after download using SHA256:
```bash
sha256sum -c metadata/checksums.sha256
