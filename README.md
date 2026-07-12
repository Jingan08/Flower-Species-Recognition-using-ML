# Flower-Species-Recognition-using-ML
A deep learning-based flower species recognition system using transfer learning and ensemble learning across multiple public flower datasets.
---
## 📖 Project Overview

Flower species recognition is a challenging image classification problem due to the high visual similarity between flower species and variations in lighting, background, viewpoint, and image quality.

This project proposes a **heterogeneous ensemble learning framework** that combines the strengths of multiple pre-trained Convolutional Neural Networks (CNNs) to achieve more accurate and robust flower classification.

Three baseline CNN models are implemented:

- VGG16
- DenseNet121
- InceptionV3

Three ensemble learning techniques are evaluated:

- Soft Voting
- Weighted Voting
- Stacking

The proposed framework is evaluated using three publicly available flower datasets with different levels of classification complexity.

---

## 🚀 Features

- Transfer Learning using ImageNet pre-trained models
- Three baseline CNN architectures
- Multiple ensemble learning strategies
- Image preprocessing and data augmentation
- Performance comparison across multiple datasets
- Automatic performance evaluation
- Confusion Matrix
- Classification Report
- Accuracy comparison charts

---

## 📂 Datasets

This project evaluates the proposed framework on three public datasets.

| Dataset | Classes |
|----------|---------:|
| Kaggle Flowers Recognition | 5 |
| TensorFlow Flowers | 5 |
| Oxford-102 Flowers | 102 |

---

## 🧠 Model Architecture

### Baseline Models

- VGG16
- DenseNet121
- InceptionV3

### Ensemble Models

- Soft Voting
- Weighted Voting
- Stacking

---

## 🔄 Project Workflow

```text
Flower Dataset
        │
        ▼
Data Preprocessing
(Image Resize, Normalization,
Data Augmentation)
        │
        ▼
Baseline CNN Models
├── VGG16
├── DenseNet121
└── InceptionV3
        │
        ▼
Ensemble Learning
├── Soft Voting
├── Weighted Voting
└── Stacking
        │
        ▼
Performance Evaluation
        │
        ▼
Accuracy Comparison
```

---

## 🛠 Libraries Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- OpenCV
- Kaggle Notebook
- Google Colab

---

## 📦 Installation

Install the required libraries.

```bash
pip install tensorflow
pip install keras
pip install numpy
pip install pandas
pip install matplotlib
pip install scikit-learn
pip install opencv-python
pip install pillow
```
---
## 📊 Experimental Results

### Kaggle Flowers Recognition Dataset

| Model | Accuracy (%) |
|------|-------------:|
| VGG16 | 82.33 |
| DenseNet121 | 90.60 |
| InceptionV3 | 91.28 |
| Soft Voting | 92.39 |
| Stacking | 92.84 |
| **Weighted Voting** | **93.06** |

---

### TensorFlow Flowers Dataset

| Model | Accuracy (%) |
|------|-------------:|
| VGG16 | 84.55 |
| DenseNet121 | 90.58 |
| InceptionV3 | 95.29 |
| Soft Voting | 96.07 |
| Weighted Voting | 96.34 |
| **Stacking** | **98.17** |

---

### Oxford-102 Flower Dataset

| Model | Accuracy (%) |
|------|-------------:|
| VGG16 | 79.13 |
| DenseNet121 | 87.58 |
| InceptionV3 | 92.42 |
| Stacking | 93.66 |
| Soft Voting | **93.79** |
| Weighted Voting | **93.79** |

---

## 🏆 Final Outcome

The proposed heterogeneous ensemble learning framework consistently outperformed the individual CNN baseline models across all datasets.

| Dataset | Best Model | Accuracy |
|----------|-----------|---------:|
| Kaggle Flowers Recognition | Weighted Voting | **93.06%** |
| TensorFlow Flowers | Stacking | **98.17%** |
| Oxford-102 Flowers | Soft Voting / Weighted Voting | **93.79%** |

The results demonstrate that combining multiple CNN architectures through ensemble learning significantly improves flower species recognition performance and model robustness.

---

## 📁 Repository Structure

```
├── Kaggle Flowers Recognition
├── TensorFlow Flowers
├── Oxford-102 Flowers
├── Models
├── README.md
```

---

## 📚 Conference Paper

**Title**

> “Comparative Analysis of Pre-trained CNN Architectures for Multiclass Flower Species Recognition”

---

## 👨‍💻 Author

**Teo Jing An**

Bachelor of Computer Science (Artificial Intelligence)

---

## 📜 License

This project is developed for academic and research purposes.
