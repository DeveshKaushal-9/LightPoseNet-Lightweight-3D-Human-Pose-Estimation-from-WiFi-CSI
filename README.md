# LightPoseNet  
### Lightweight 3D Human Pose Estimation from WiFi CSI

LightPoseNet is a real-time wireless perception system that estimates 3D human pose using commodity WiFi Channel State Information (CSI).

This project explores low-cost, privacy-preserving alternatives to camera-based perception for robotics, smart environments, and human-aware autonomous systems.

Unlike vision-based systems, LightPoseNet:

- Works through walls  
- Preserves visual privacy  
- Operates in low-light or occluded environments  
- Runs in real time (4.1 ms inference)  
- Uses only 0.29M parameters  

---

## 🚀 Motivation

Most robotic perception systems rely heavily on cameras or LiDAR. However:

- Cameras raise privacy concerns  
- Visual systems fail under occlusion or poor lighting  
- Hardware costs can scale quickly  

WiFi signals are already present in most indoor environments.  
This work investigates whether wireless channel distortions caused by human motion can be decoded into meaningful 3D pose information.

LightPoseNet demonstrates that commodity WiFi infrastructure can function as a spatial sensing layer for intelligent systems.

---

## 🧠 System Overview

The full pipeline consists of:

WiFi CSI Acquisition → Signal Preprocessing → Feature Representation → Lightweight CNN → 3D Pose Regression

### 1️⃣ CSI Signal Processing
- Raw Channel State Information extraction  
- Noise filtering and normalization  
- Temporal window segmentation  

### 2️⃣ Feature Learning
- Lightweight convolutional architecture  
- Squeeze-and-Excitation (SE) attention variant  
- Optimized for low parameter count and fast inference  

### 3️⃣ Pose Regression
- Direct regression of 3D joint coordinates  
- Evaluation using MPJPE and PCK metrics  

---

## 📊 Results (WiPose Dataset)

| Model        | MPJPE (mm) | PCK@0.10 | Params (M) | Inference (ms) |
|-------------|------------|----------|------------|----------------|
| Baseline    | 40         | 92.88%   | 0.13       | 2.8            |
| SE-Enhanced | 40         | 93.31%   | 0.29       | 4.1            |

### Key Highlights

- ~300× parameter reduction compared to prior CSI-based approaches  
- Real-time inference suitable for edge deployment  
- Competitive accuracy with significantly lower computational cost  

---

## 📂 Dataset

This project uses the publicly available **WiPose dataset**.

The dataset is not included in this repository due to licensing constraints.

Please download the dataset from the official WiPose source and place it in the appropriate directory before running experiments.

---

## 🛠 Installation

Clone the repository:

```bash
git clone https://github.com/DeveshKaushal-9/LightPoseNet-Lightweight-3D-Human-Pose-Estimation-from-WiFi-CSI.git
cd LightPoseNet-Lightweight-3D-Human-Pose-Estimation-from-WiFi-CSI

---

## 🏅 Academic Recognition

- 🎤 **Oral Presentation** — MIT Undergraduate Research Technology Conference (URTC) 2025  
- 🧠 **Poster Accepted** — AAAI 2026 Empowering Global South AI (EGSAI) Workshop, Singapore  
- 🏆 **Finalist** — TechConnect’25 Research Poster Competition (ResCon), IIT Bombay  

---

## 📄 Citation

If you use this work, please cite:

**Lightweight Human Pose Estimation from WiFi Channel State Information Using Deep Neural Networks**  
MIT URTC 2025  

(PDF available in repository)

---

## 👤 Author

**Devesh Kaushal**  
B.Tech, Computer Science & Engineering  

Research interests:  
Wireless sensing, real-time perception, efficient deep learning, and AI systems for physical-world intelligence.

---

## 📜 License

MIT License
