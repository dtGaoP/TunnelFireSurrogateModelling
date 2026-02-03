# TunnelFireSurrogateModelling
# TunnelFire180 Dataset (FDS-based)

This repository provides the metadata, documentation, and access links for the tunnel fire temperature-field dataset used in our paper:
**"[Physics-informed Fourier neural operator for surrogate prediction of tunnel fire temperature field]"** (2026).

> **Note:** Due to the large size of the raw data, the dataset files are hosted on Baidu Netdisk. This GitHub repository contains documentation, metadata, checksums, and minimal loading examples.

---

## Dataset Overview
- Simulator: Fire Dynamics Simulator (FDS) v6.7
- Geometry: Tunnel length [100 m], height [7.2 m], width [6 m] (2D slice via 1 cell in transverse direction)
- Ambient: 20 °C, 101.325 kPa
- Outputs: temperature **T**, longitudinal velocity **U**, vertical velocity **W**
- Sampling: Δt = 1 s, total frames = 601 (0–600 s)
- Grid: H × W = 19 × 251 (z × x) 
- Global conditions: PHRR (MW), fire location xf (m), ventilation velocity v_vent (m/s), tunnel slope (%)

---

## Code availability
The training and inference code will be released soon in this repository.

---

## Results

We provide two lightweight GIF demos for quick visualization.

### Demo 1 — 30MW, 20m, 0m/s, 3%
<p align="center">
  <img src="results/Video S1.gif" width="900" alt="Demo 1">
</p>

### Demo 2 — 5MW, 20m, 2m/s, -3%
<p align="center">
  <img src="results/Video S2.gif" width="900" alt="Demo 2">
</p>

**Notes**
- The GIFs are intended for qualitative inspection (visual structure, plume boundary, hotspot location).
- Quantitative metrics and additional cases are reported in the paper.

---

## Download
### Baidu Netdisk
- File: `scenario_180.zip`
- Link: https://pan.baidu.com/s/14tJ3ByrnQU2V_xYXLT-1dQ
- Extraction code (提取码): **2309**

**Recommended:** Verify file integrity after download using SHA256:
```bash
sha256sum -c metadata/checksums.sha256
