# 👁️ smartAFNET – Eye Refraction Error Detection Model

A deep learning–based eye refraction error detection model built using transfer learning (ResNet50 + REDNet), designed for single-image inference and optimized for TensorFlow Lite mobile deployment.

---

## 📌 Overview

This repository contains the deep learning model and training pipeline for detecting eye refraction errors from a single eye image.

The model leverages transfer learning with ResNet50, a REDNet-inspired architecture with skip connections, and Grad-CAM visualization for interpretability. Trained weights are later converted to TensorFlow Lite for deployment in a separate Android mobile application.

---

## 🚀 Features

- 🧠 Transfer learning with ResNet50 backbone  
- 🔁 REDNet-inspired encoder–decoder architecture with skip connections  
- 🔒 Frozen base layers for stable feature extraction  
- 🔥 ReLU6 activation for mobile-efficient inference  
- 🎯 Grad-CAM heatmap visualization for interpretability  
- 📦 TensorFlow Lite (TFLite) export for mobile deployment  
- 🖼️ Single-image inference support

---

## 🧠 Model Architecture

### Backbone
- ResNet50 (pretrained on ImageNet)
- Base layers frozen

### Custom Head (REDNet-inspired)
- Encoder–decoder structure
- Skip connections
- ReLU6 activations

### Explainability
- Grad-CAM heatmaps highlight important eye regions used for predictions

---

## 🛠️ Tech Stack

- Python
- TensorFlow / Keras
- ResNet50
- REDNet
- Grad-CAM
- NumPy
- Matplotlib
- OpenCV
- TensorFlow Lite (TFLite)
- Android (Java)

---

## 📂 Project Structure

smartAFNET/
│
├── smartAFNet2_0.ipynb # Training & experimentation notebook
├── .gitignore
├── README.md
├── LICENSE


---

## ⚙️ Installation

```bash
pip install tensorflow numpy matplotlib opencv-python pillow
```

## ▶️ How to Run

### Jupyter / VS Code
```bash
jupyter notebook smartAFNet2_0.ipynb
```

### Google Colab
```bash
Upload the notebook and run all cells.
```

## 📊 Training Pipeline
Load and preprocess eye images

Apply transfer learning with ResNet50

Freeze backbone layers

Train REDNet-based head with skip connections

Optimize with ReLU6

Generate Grad-CAM visualizations

Convert to TensorFlow Lite

Deploy to Android app

## 📸 Inference Workflow
Camera → Capture Eye Image → TFLite Model → Prediction → Result + Heatmap
Runs offline

Fast on-device inference

Privacy-friendly (no server upload)

## 📈 Applications
Vision screening assistance

Preliminary refraction error detection

Educational/clinical research

Edge AI healthcare solutions

## 👥 Contributors
John Audrey L. Cansino

Carl Angelo L. Cruzpero

Mark Russel M. De Jesus

Erika Gabrielle A. Madrid

Alveen Keith M. Sareno

## 📜 License
MIT License


---
