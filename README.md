# AUDRON: Drone Type Recognition Using Acoustic Signals 🚁🔊

AUDRON (AUdio-based Drone Recognition Network) is a **deep learning framework for drone type recognition using acoustic signals**. The system leverages **fused audio feature representations** to robustly distinguish drone sounds from background noise and classify different drone types, even under challenging real-world conditions.

📄 **arXiv Paper**: https://arxiv.org/abs/2512.20407  

🎤 **Presented at the flagship conference**:  
**IEEE INDICON 2025 (22nd IEEE India Council International Conference)** —  
*Regenerative Artificial Intelligence: Advancing AI for Industrial, Societal, and Environmental Impact*

---

## 🧠 Model Architecture

The overall architecture of the proposed AUDRON framework is shown below:

![AUDRON Architecture](architecture.png)

AUDRON employs a **multi-branch hybrid architecture** with feature-level fusion for reliable acoustic drone detection.

---

## 📌 Project Overview

- 🎧 Drone detection and classification using **audio-only sensing**
- 🧠 Hybrid deep learning framework with **multiple acoustic representations**
- 🔀 Feature-level fusion for improved robustness
- 🧪 Evaluated on **binary and multiclass** classification tasks
- 📊 Achieves high accuracy under real-world noise conditions

---

## 📂 Repository Contents

- `AUDRON_Drone_Type_Classification(Binary_with_No_Augmentation).ipynb`  
  Binary classification experiment without data augmentation

- `drone-type-classification-using-drone-audio-sound.ipynb`  
  Complete pipeline for feature extraction, training, and evaluation

- `INDICON PRESENTATION 2025.pptx`  
  Conference presentation slides (IEEE INDICON 2025)

- `architecture.png`  
  Architecture diagram of the AUDRON framework

---

## 🧪 Methodology

- **Acoustic Data**
  - Real drone audio from DroneAudioDataset
  - Environmental noise from ESC-50, Speech Commands, and silence clips
  - Synthetic drone audio generation for quadcopter, hexacopter, octocopter, and racing drones

- **Feature Extraction (Parallel Branches)**
  - MFCCs processed using a 1D CNN
  - STFT spectrograms processed using a 2D CNN
  - Temporal modeling using BiLSTM with attention
  - Autoencoder-based latent audio representations

- **Architecture & Fusion**
  - Four-branch multi-modal architecture
  - Feature-level fusion via concatenation

---
## 🧠 Applications

- Airspace surveillance
- Security and defense monitoring
- Detection of unauthorized drones
- Smart city and autonomous sensing systems

---

## 📜 Citation

If you use this work in your research, please cite:

```bibtex
@article{chatterjee2025audron,
  title={AUDRON: A Deep Learning Framework with Fused Acoustic Signatures for Drone Type Recognition},
  author={Chatterjee, Rajdeep and Chakrabarty, Sudip and Acharjee, Trishaani and Mishra, Deepanjali},
  journal={arXiv preprint arXiv:2512.20407},
  year={2025}
}
