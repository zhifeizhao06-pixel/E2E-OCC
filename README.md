# E2E-OCC

# Semantic-AD

This repository provides visual demonstrations and supplementary materials for the paper:

**Interpretable and Generalizable Diffusion Planning via Vision-Language Guidance and Agent-Aware Trajectory Initialization**

**Code will be released upon acceptance.**

---

## 📣 Overview

We propose a vision-language guided diffusion planning framework for autonomous driving, integrating:

- **High-level semantic driving instructions** extracted using a Vision-Language Model (Qwen2.5-VL)
- **Agent-aware spatial distribution cues** projected onto a BEV map
- **Dynamic trajectory initialization** for more structured, adaptive diffusion sampling
- **Conditional diffusion decoding** that improves interpretability, rationality, and intent alignment

Our framework significantly enhances **generalizability**, **safety**, **interpretability**, and **trajectory consistency** across complex driving scenarios.

---

## 🏛️ Framework Overview

<p align="center">
  <img src="assets/main_framework.png" width="900">
</p>

**Figure:** Overview of our language-guided diffusion planner.  
The architecture fuses multi-modal perception (RGB, LiDAR), vehicle state, learned semantic cues, and agent-aware priors to guide diffusion-based trajectory generation.

---

## 🚗 Qualitative Results

### 1. Comparison with Baselines

<p align="center">
  <img src="assets/qualitative_compare.png" width="900">
</p>

**Figure:** Comparison with representative baseline planners.  
Our method produces more consistent, scene-aware, and drivable trajectories (red = prediction, green = ground truth).

---

### 2. Vision-Language Guidance (Ablation Example)

<p align="center">
  <img src="assets/vlm_guidance.png" width="700">
</p>

**Figure:** Examples illustrating the effect of VLM semantic priors (e.g., “turn left”, “follow the lane”, “slow down”).  
Semantic cues enforce stronger intent consistency and reduce ambiguous planning behaviors.

---

### 3. Interaction-Aware Conflict Handling (DIFM)

<p align="center">
  <img src="assets/conflict_detection.png" width="700">
</p>

**Figure:** Our DIFM module resolves conflicts between semantic direction (`f_dir`) and interaction fields (`f_interact`), improving safety around dynamic agents.

---

## 📊 Quantitative Summary

Below is a sample table (replace values with your own or substitute with a figure such as `assets/table_results.png`):

| Method         | NC ↑  | DAC ↑ | TTC ↑ | Comf. ↑ | EP ↑  | PDMS ↑ |
|----------------|-------|-------|-------|---------|-------|--------|
| TransFuser     | 97.7  | 92.8  | 92.8  | 100     | 79.2  | 84.0   |
| DiffusionDrive | 98.2  | 96.2  | 94.7  | 100     | 82.2  | 88.1   |
| **Ours**       | **99.3** | **96.4** | **96.5** | **100** | **84.5** | **90.4** |

---

## 📁 Recommended Project Structure

```
Semantic-AD/
│── README.md
│── assets/
│   ├── main_framework.png            # main architecture
│   ├── qualitative_compare.png       # qualitative comparison
│   ├── vlm_guidance.png              # semantic guidance examples
│   ├── conflict_detection.png        # DIFM ablation
│   ├── table_results.png             # optional: result table figure
│   └── ... (additional figures)
└── (code to be released)
```

---

## 📄 Paper

**Title:** Interpretable and Generalizable Diffusion Planning via Vision-Language Guidance and Agent-Aware Trajectory Initialization  
**Authors:** Ran Bu, Junjie Zhang, Qirong Liu, Liang Song, Zhifei Zhao, Yanzi Miao  
**Status:** Under Review  
**Preprint:** Available in project resources.

---

## 📬 Contact

If you have any questions or need additional materials:

**Email:** your_email@domain.com

---

## 🔒 Code Availability

The full implementation is currently under review and will be released once the paper is accepted.

---

If you'd like, I can also:

- Export figures from your PDF into the `assets/` folder
- Produce a dark-mode or banner-enhanced README
- Generate an OpenGraph banner for GitHub previews

Just tell me which task to do next.
