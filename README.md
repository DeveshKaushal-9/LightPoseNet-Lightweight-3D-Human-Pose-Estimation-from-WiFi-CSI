# LightPoseNet
### Lightweight 3D Human Pose Estimation from WiFi CSI

Official implementation of the research work:

**"Lightweight Human Pose Estimation from WiFi Channel State Information Using Deep Neural Networks"**

---

## 🏅 Academic Recognition

- 🎤 Oral Presentation — MIT Undergraduate Research Technology Conference (URTC) 2025
- 🧠 Poster Accepted — AAAI 2026 Empowering Global South AI (EGSAI) Workshop, Singapore
- 🏆 Finalist — TechConnect’25 Research Poster Competition (ResCon), IIT Bombay

---

## 📄 Overview

LightPoseNet is a lightweight convolutional neural network (CNN) framework for privacy-preserving 3D human pose estimation using WiFi Channel State Information (CSI).

Unlike vision-based systems, this approach:
- Works through walls
- Preserves visual privacy
- Runs in real time (4.1 ms inference)
- Uses only 0.29M parameters

---

## 📊 Results (WiPose Dataset)

| Model | MPJPE (mm) | PCK@0.10 | Params (M) | Inference (ms) |
|-------|------------|----------|------------|----------------|
| Baseline | 40 | 92.88% | 0.13 | 2.8 |
| SE-Enhanced | 40 | 93.31% | 0.29 | 4.1 |

---

## 📂 Dataset

This work uses the publicly available WiPose dataset.
The dataset is not included in this repository.

---

