# E2E-OCC


This repository provides visual demonstrations and supplementary materials for the paper:

**E2EOcc: End-to-End 4D Occupancy World Modeling with Unified Spatiotemporal Diffusion**

**Code will be released upon acceptance.**
<p align="center">
  <img src="image/f2.jpg" width="900">
</p>

---

## 📣 Overview
We propose an integrated training scheme that jointly optimizes occupancy feature extraction and latent spatiotemporal modeling via diffusion, mitigating the information bottleneck of conventional VAE-based methods and enhancing the model’s performance:

- **We design a novel feature extraction network tailored for dynamic scene modeling, which adapts to 4D discrete voxel representations and improves feature retention in sparse environments.** 
- **We introduce a diffusion training paradigm augmented by dynamic distillation to balance performance and efficiency, accelerating convergence and boosting feature robustness.**


---

## 🏛️ Framework Overview

<p align="center">
  <img src="image/f1.png" width="900">
</p>

**Figure:** Overview of our language-guided diffusion planner.  
The architecture fuses multi-modal perception (RGB, LiDAR), vehicle state, learned semantic cues, and agent-aware priors to guide diffusion-based trajectory generation.

---

## 🚗 Qualitative Results

### 1. Comparison with Baselines

<p align="center">
  <img src="image/f4.jpg" width="900">
</p>

**Figure:** Comparison with representative baseline planners.  
Our method produces more consistent, scene-aware, and drivable trajectories (red = prediction, green = ground truth).

---





## 📊 Quantitative Summary

Below is a sample table (replace values with your own or substitute with a figure such as `assets/table_results.png`):

| Method         | NC ↑  | DAC ↑ | TTC ↑ | Comf. ↑ | EP ↑  | PDMS ↑ |
|----------------|-------|-------|-------|---------|-------|--------|
| TransFuser     | 97.7  | 92.8  | 92.8  | 100     | 79.2  | 84.0   |
| DiffusionDrive | 98.2  | 96.2  | 94.7  | 100     | 82.2  | 88.1   |
| **Ours**       | **99.3** | **96.4** | **96.5** | **100** | **84.5** | **90.4** |

---



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
