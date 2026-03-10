# ⚡ AI-Based Detection and Self-Healing of False Data Injection Attacks (FDIA) in Smart Grids

## Overview

This project presents an **AI-driven cybersecurity framework for smart grids** capable of detecting and repairing **False Data Injection Attacks (FDIA)** in power system sensor data.

Smart grids rely heavily on sensor measurements to maintain stable and efficient power distribution. However, these systems are vulnerable to cyberattacks that manipulate sensor data and disrupt grid operations.

This project introduces an intelligent pipeline that combines:

* **Machine learning attack detection**
* **Explainable AI for transparency**
* **Autoencoder-based self-healing**

The goal is to create **resilient, secure, and sustainable power systems** capable of automatically responding to cyber threats.

---

# Project Architecture

Smart Grid Sensor Data
↓
Random Forest Attack Detection
↓
Explainable AI (SHAP)
↓
Autoencoder Reconstruction
↓
Self-Healing Smart Grid Data

---

# Key Features

## 1️⃣ FDIA Attack Detection

A **Random Forest classifier** is trained on smart grid sensor measurements to classify system states into:

* Normal operation
* Natural disturbances
* False Data Injection Attacks

Performance:

* **Test Accuracy:** ~92%
* **Precision / Recall / F1:** Above 0.9 for most classes

This enables reliable identification of malicious manipulation of grid sensor data.

---

## 2️⃣ Explainable AI (XAI)

To improve trust and interpretability, the project integrates **SHAP (SHapley Additive Explanations)**.

Capabilities include:

* Feature importance visualization
* Local explanations for individual predictions
* Identification of the sensors most responsible for attack detection

This helps **grid operators understand why the AI flagged an attack**.

---

## 3️⃣ Self-Healing AI

The project introduces an **autoencoder-based repair system** trained on normal grid data.

When attacks corrupt sensor values:

* The autoencoder reconstructs the expected normal values.
* Malicious spikes are suppressed.
* Sensor readings return to normal operational ranges.

Performance:

* **Average reconstruction error:** ~0.00058 (scaled data)

This demonstrates the ability of AI to **repair compromised sensor signals in real time**.

---

# Visualizations

The project includes several visualizations to demonstrate system behavior:

* Original sensor signals
* Corrupted signals during attacks
* Repaired sensor values after AI reconstruction
* Reconstruction error highlighting attack locations
* SHAP feature importance plots

These plots clearly show the **self-healing behavior of the system**.

---

# Applications

This research has applications in:

* Smart grid cybersecurity
* Real-time energy system monitoring
* AI-driven cyber-physical system protection
* Sustainable energy infrastructure
* Utility operator decision support

---

# Project Structure

```
fdia-smart-grid-ai
│
├── README.md
├── requirements.txt
├── LICENSE
│
├── data/
│   └── smart_grid_sensor_data.csv
│
├── notebooks/
│   └── fdia_detection_self_healing.ipynb
│
├── models/
│   ├── rf_fdia_detector.pkl
│   └── autoencoder_model.h5
│
└── results/
    ├── shap_feature_importance.png
    ├── reconstruction_error.png
    └── sensor_repair_visualization.png
```

---

# Technologies Used

Python
Machine Learning
Explainable AI
Smart Grid Data Analytics

Libraries:

* scikit-learn
* TensorFlow / Keras
* SHAP
* pandas
* numpy
* matplotlib

---

# Future Improvements

Potential extensions include:

* Real-time attack detection dashboard
* Attack localization across multiple sensors
* Graph Neural Networks for topology-aware detection
* Deployment within digital twin smart grid simulations

---

# Author

**Meenu Hani**

AI • Cybersecurity • Energy Analytics

---

# License

This project is protected under a custom license.
Permission from the author is required before any use or distribution.

