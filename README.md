# Transformer Differential Relay (TDR) Dataset: Faults and FDIAs

This repository provides a comprehensive dataset of three-phase current measurements collected by a **Transformer Differential Relay (TDR)** under both **legitimate electrical faults** and **false data injection attacks (FDIAs)**.

📂 Dataset: [https://github.com/AhmadMSGit/Data](https://github.com/AhmadMSGit/Data)

---

## 📁 Dataset Structure

The dataset contains **53,490** multivariate time-series samples, organized into six subfolders:

- `one_phase_to_ground_faults/`
- `two_phase_to_ground_faults/`
- `three_phase_to_ground_faults/`
- `one_phase_to_ground_attacks/`
- `two_phase_to_ground_attacks/`
- `three_phase_to_ground_attacks/`

Each subfolder corresponds to a specific fault type or FDIA scenario. Each file represents a single event recorded by the TDR.

---

## 📊 Data Format

- **Channels**: 6 (Three-phase currents from both sides of the transformer)
- **Sampling Rate**: 4800 samples/second  
- **Window Duration**: 20 milliseconds (96 time steps per channel)
- **Time Alignment**: Window begins ~10 ms before the fault or attack event
- **Format**: .pkl files, each of shape `(6, 96)` — 6 channels × 96 time steps

---

## ⚡ Event Types

### ✅ Legitimate Fault Scenarios
Simulated fault conditions to represent realistic power system events:
- Single-phase (1Φ), two-phase (2Φ), and three-phase (3Φ) faults
- Varying inception angles, durations, and locations

### 🚨 FDIA Scenarios
Simulated cyberattacks aiming to deceive the relay into misclassifying an attack as a fault:
- **Magnitude Manipulation**
- **Phase Angle Manipulation**
- **Time-Synchronization Attacks**
- Targeting 1, 2, or all 3 phases with randomized start times and durations

---

## 🧪 Simulation Details

- **Test System**: IEEE PSRC D6 Benchmark Test System  
- **Platform**: OPAL-RT HYPERSIM (real-time digital simulator)  
- **Standard**: Data collected with a sampling rate in compliance with IEC 61850-9-2

---

## 🧠 Applications

This dataset is ideal for developing and benchmarking:
- Transformer protection schemes
- Cyberattack detection and mitigation models
- Deep learning and time-series classification techniques
- Research on TDR response under cyber-physical threats

---

## 📄 Citation

If you use this dataset in your research, please cite the following:

> Ahmad Mohammad Saber, Hany E. Z. Farag, Amr Youssef and Deepa Kundur, “A Model-Independent Trojan Attack on Deep Learning-Based FDIA Detection in Smart Grid Protection Systems”, Submitted, 2025.  
> Dataset: [https://github.com/AhmadMSGit/Data](https://github.com/AhmadMSGit/Data)

---

For questions or contributions, please email ahmad.m.saber@ieee.org or dkundur@comm.utoronto.ca


---

## ⚠️ Important Note

Due to GitHub's file size limitations, **a portion of the dataset could not be uploaded here**.  
You can access the full dataset from Google Drive:

🔗 **[Complete Dataset on Google Drive](https://drive.google.com/drive/folders/1s6XiRNGMsqEqWaiSUVn4D7lv-GEOTWjN?usp=sharing)**

---
