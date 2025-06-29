# 🌿 Crop Disease Detection using CNN and Transfer Learning

This repository contains a machine learning project for detecting crop diseases from leaf images using the **PlantVillage dataset**. Three models were developed and evaluated: a custom-built CNN, and two pretrained models—**ResNet50** and **Xception**. The models classify plant leaves as **healthy** or **diseased**, supporting early and accurate diagnosis in agriculture.

---

## 📂 Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Model Summaries](#model-summaries)
- [Installation](#installation)
- [How to Run](#how-to-run)
- [Results](#results)
- [Limitations & Future Work](#limitations--future-work)
- [References](#references)
- [License](#license)
- [Author](#author)

---

## 📜 Overview

The project explores different deep learning approaches to classify plant leaf images. A baseline CNN model was trained from scratch, and two advanced architectures (ResNet50 and Xception) were fine-tuned using transfer learning to compare performance.

---

## 🛠 Tech Stack

- Python
- TensorFlow / Keras
- Jupyter Notebook
- Matplotlib / Seaborn
- NumPy / Pandas
- Git & GitHub

---

## 🌱 Dataset

- **Name**: [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
- **Type**: Image dataset of healthy and diseased plant leaves
- **Classes**: Multiple disease categories and healthy leaves
- **Images**: ~50,000 RGB images

---

## Model Summaries

| Model               | Training Accuracy | Validation Accuracy |
|---------------------|-------------------|----------------------|
| CNN (from scratch)  | 98.59%            | 96.01%               |
| ResNet50 (Pretrained) | 99.66%            | 96.58%               |
| Xception (Pretrained) | 78.02%            | 68.82%               |

- ✅ **CNN**: Custom architecture with Conv2D, MaxPooling, Dropout, and Dense layers.
- 🔁 **ResNet50**: Transfer learning with pretrained ImageNet weights.
- ⚠️ **Xception**: Underperformed—possibly due to overfitting or learning rate issues.

---

## 💾 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/crop-disease-detection.git
   cd crop-disease-detection
