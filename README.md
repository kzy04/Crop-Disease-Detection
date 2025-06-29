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


## ▶️ How to Run

Open and run any of the following Jupyter Notebooks:

- **CNN Model (from scratch)**:  
  `cnn_model.ipynb`

- **ResNet50 (Transfer Learning)**:  
  `resnet50_model.ipynb`

- **Xception (Transfer Learning)**:  
  `xception_model.ipynb`

Each notebook includes:
- Data preprocessing
- Model architecture
- Training and validation
- Accuracy & loss visualizations

---

## 📈 Results

The best-performing model was **ResNet50**, achieving a validation accuracy of **96.58%**.

Training and validation curves are visualized within each notebook.

| Model               | Training Accuracy | Validation Accuracy |
|---------------------|-------------------|----------------------|
| CNN (from scratch)  | 98.59%            | 96.01%               |
| ResNet50 (Pretrained) | 99.66%            | 96.58%               |
| Xception (Pretrained) | 78.02%            | 68.82%               |

---

## ⚠️ Limitations & Future Work

- Performance may vary on real-world, noisy, or unseen crop images.
- Current models trained on clean, labeled dataset images.
- **Future enhancements**:
  - Data augmentation to improve generalization
  - Real-world image testing
  - Mobile deployment with TensorFlow Lite
  - Web or mobile interface integration (e.g., Streamlit or Flutter)

---

## 🔗 References

- [PlantVillage Dataset](https://www.kaggle.com/datasets/emmarex/plantdisease)
- [Keras Applications Models](https://keras.io/api/applications/)

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Junaid Hossain**  
GitHub: [@kzy04](https://github.com/kzy04)

Feel free to open issues or contribute to this project!
