# 🌸 Flower Species Recognition using Heterogeneous Ensemble Learning

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange)
![Keras](https://img.shields.io/badge/Keras-Deep%20Learning-red)
![Status](https://img.shields.io/badge/Status-Completed-success)

</p>

A deep learning-based flower species recognition system using **Transfer Learning** and **Heterogeneous Ensemble Learning** with **VGG16**, **DenseNet121**, and **InceptionV3**.

---

# 📖 Project Overview

This project investigates the effectiveness of **heterogeneous ensemble learning** for flower species recognition.

Instead of relying on a single CNN architecture, this project combines the prediction outputs of multiple deep learning models to improve classification accuracy and robustness.

The framework is evaluated using **three public flower datasets** with different classification complexities.

---

# 🎯 Project Objectives

✅ Develop a flower species recognition system using transfer learning.

✅ Implement heterogeneous ensemble learning.

✅ Compare Soft Voting, Weighted Voting and Stacking.

✅ Evaluate the proposed framework on multiple public datasets.

---

# 🌼 Datasets

| Dataset | Classes | Purpose |
|----------|---------:|----------------|
| 🌸 Kaggle Flowers Recognition | 5 | Simple classification |
| 🌼 TensorFlow Flowers | 5 | Balanced dataset |
| 🌺 Oxford-102 Flowers | 102 | Fine-grained classification |

---

# 🧠 Models

## Baseline CNN

- ✅ VGG16
- ✅ DenseNet121
- ✅ InceptionV3

## Ensemble Learning

- Soft Voting
- Weighted Voting
- Stacking

---

# 🔄 Workflow

```text
Flower Dataset
        │
        ▼
Preprocessing
(Resize • Normalize • Augmentation• Splitting)
        │
        ▼
Feature Extraction
Using Baseline CNN Models
(VGG16 • DenseNet121 • InceptionV3)
        │
        ▼
Output Prediction 
        │
        ▼
Ensemble Learning
(Soft Voting • Weighted Voting • Stacking)
        │
        ▼
Performance Evaluation
        │
        ▼
Accuracy Comparison
```

## 📁 Repository Structure

```
├── SourceCode/
│   │
│   ├── Model/
│   │   ├── Kaggle Flowers/
│   │   ├── TensorFlow Flowers/
│   │   └── Oxford-102 Flowers/
│   │
│   └── Code/
│       │
│       ├── Model_Training/
│       │   ├── Kaggle Flowers.ipynb
│       │   ├── TensorFlow Flowers.ipynb
│       │   └── Oxford-102 Flowers.ipynb
│       │
│       └── EnsembleModel_Implementation/
│           ├── Kaggle Flowers.ipynb
│           ├── TensorFlow Flowers.ipynb
│           └── Oxford-102 Flowers.ipynb
```
| Folder                           | Description                                                                                                                                                                                                                                                |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Model**                        | Contains the trained CNN models (.keras/.h5) for each dataset. These models are used by the ensemble implementation and do not need to be retrained unless required.                                                                                       |
| **Code**                         | Contains all Jupyter Notebook (`.ipynb`) source code used in this project.                                                                                                                                                                                 |
| **Model_Training**               | Contains the notebooks for training the baseline CNN models (VGG16, DenseNet121, and InceptionV3) separately for each dataset. Running these notebooks will generate the trained model files stored in the **Model** folder.                               |
| **EnsembleModel_Implementation** | Contains the notebooks for implementing the proposed ensemble learning methods (Soft Voting, Weighted Voting, and Stacking). These notebooks load the trained models from the **Model** folder and perform ensemble prediction and performance evaluation. |

---

# 📊 Experimental Results

## 🌸 Kaggle Flowers

| Model | Accuracy |
|------|---------:|
| VGG16 | 82.33% |
| DenseNet121 | 90.60% |
| InceptionV3 | 91.28% |
| Soft Voting | 92.39% |
| Stacking | 92.84% |
| 🥇 **Weighted Voting** | **93.06%** |

---

## 🌼 TensorFlow Flowers

| Model | Accuracy |
|------|---------:|
| VGG16 | 84.55% |
| DenseNet121 | 90.58% |
| InceptionV3 | 95.29% |
| Soft Voting | 96.07% |
| Weighted Voting | 96.34% |
| 🥇 **Stacking** | **98.17%** |

---

## 🌺 Oxford-102 Flowers

| Model | Accuracy |
|------|---------:|
| VGG16 | 79.13% |
| DenseNet121 | 87.58% |
| InceptionV3 | 92.42% |
| Stacking | 93.66% |
| 🥇 Soft Voting | **93.79%** |
| 🥇 Weighted Voting | **93.79%** |

---

# 🏆 Final Performance

| Dataset | Best Model | Accuracy |
|---------|-----------|---------:|
| 🌸 Kaggle Flowers | Weighted Voting | **93.06%** |
| 🌼 TensorFlow Flowers | Stacking | **98.17%** |
| 🌺 Oxford-102 Flowers | Soft Voting / Weighted Voting | **93.79%** |

---

# ⭐ Key Achievements

- ✅ Evaluated **3 public flower datasets**
- ✅ Compared **3 transfer learning CNN models**
- ✅ Implemented **3 ensemble learning techniques**
- ✅ Achieved **98.17% classification accuracy**
- ✅ Outperformed previous studies across all datasets

---

# 📂 Repository Structure

```text
📦 Flower-Species-Recognition-using-ML
│
├── 📁 Kaggle Flowers
├── 📁 TensorFlow Flowers
├── 📁 Oxford-102 Flowers
└── README.md
```

---

# 📑 Conference Paper

**Title**

> Comparative Analysis of Pre-trained CNN Architectures for Multiclass Flower Species Recognition

---

# 👨‍💻 Author

**Teo Jing An**

---

# ⭐ If you find this project useful, please consider giving it a star!
