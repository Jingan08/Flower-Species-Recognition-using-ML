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

| Dataset | Classes | Purpose | Dataset Link |
|----------|---------:|----------------|-----------------------------|
| 🌸 Kaggle Flowers Recognition | 5 | Simple classification | https://www.kaggle.com/datasets/alxmamaev/flowers-recognition/data |
| 🌼 TensorFlow Flowers | 5 | Balanced dataset | http://download.tensorflow.org/example_images/flower_photos.tgz |
| 🌺 Oxford-102 Flowers | 102 | Fine-grained classification | https://www.robots.ox.ac.uk/~vgg/data/flowers/102/ |

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

## 📁 Repository Structure & Notebook Links

Since Jupyter Notebooks with outputs are often too large to render directly on GitHub, you can use the **nbviewer** links below to view the notebooks with all outputs, training charts, and evaluation results fully visible.

### 🧠 Model Training Notebooks
These notebooks are used to train the baseline CNN models (VGG16, DenseNet121, and InceptionV3) for each dataset.

| Notebook | Dataset | Render Link (with outputs) |
| :--- | :---: | :---: |
| 🌸 `kaggledataset-trainmodel.ipynb` | Kaggle Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/ModelTraining/kaggledataset-trainmodel.ipynb) |
| 🌼 `tensorflowdataset-trainmodel.ipynb` | TensorFlow Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/ModelTraining/tensorflowdataset-trainmodel.ipynb) |
| 🌺 `oxford-102-trainmodel.ipynb` | Oxford-102 Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/ModelTraining/oxford-102-trainmodel.ipynb) |

### 🔄 Ensemble Implementation Notebooks
These notebooks implement the proposed ensemble learning methods (Soft Voting, Weighted Voting, and Stacking) using the trained baseline models.

| Notebook | Dataset | Render Link (with outputs) |
| :--- | :---: | :---: |
| 🌸 `kaggledataset-ensemble.ipynb` | Kaggle Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/EnsembleModel_Implementation/kaggledataset-ensemble.ipynb) |
| 🌼 `ensemble-tensorflowdataset.ipynb` | TensorFlow Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/EnsembleModel_Implementation/ensemble-tensorflowdataset.ipynb) |
| 🌺 `ensemble-oxford-102.ipynb` | Oxford-102 Flowers | [![nbviewer](https://img.shields.io/badge/render-nbviewer-orange.svg)](https://nbviewer.org/github/Jingan08/Flower-Species-Recognition-using-ML/blob/main/EnsembleModel_Implementation/ensemble-oxford-102.ipynb) |

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


# 📑 Conference Paper

**Title**

> Comparative Analysis of Pre-trained CNN Architectures for Multiclass Flower Species Recognition

---

# 👨‍💻 Author

**Teo Jing An**

---

# ⭐ If you find this project useful, please consider giving it a star!
