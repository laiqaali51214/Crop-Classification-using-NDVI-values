
# 🌾🧵 ML Crop Classification: Rice vs Cotton 

An interactive guide to explore the ML project classifying rice and cotton crops using NDVI data (2021-2023).  
**Click sections below** to navigate!

<details>
<summary><strong>📌 Table of Contents</strong></summary>

1. [Project Overview](#-project-overview)  
2. [Key Features](#-key-features)  
3. [Installation](#-installation)  
4. [Workflow Summary](#-workflow-summary)  


</details>

---

## 🚀 Project Overview
**Goal:** Classify rice (Class `1`) and cotton (Class `0`) using NDVI values from 12 monthly observations.  
**Data:**  
- 3 years of data (2021, 2022, 2023) for both crops.  
- 12 NDVI features (`NDVI01` to `NDVI12`) + `Class` label.  

---

## 🌟 Key Features
- **Data Preprocessing:**  
  - Handling duplicates, outliers (Z-score, Isolation Forest).  
  - Class balancing (SMOTE, Random Over/Undersampling).  
  - Feature scaling (PowerTransform + Standardization).  
- **EDA:** Time-series analysis, correlation matrices, univariate/bivariate plots.  
- **Models:**  
  - Supervised: XGBoost, Random Forest, SVM, Bagging.  
  - Unsupervised: K-Means, Hierarchical Clustering.  
- **Hyperparameter Tuning:** GridSearchCV for optimal parameters.  

---

## 💻 Installation
```bash
!pip install xgboost scikit-learn==1.5.0 pandas numpy matplotlib seaborn imbalanced-learn
```

---

## 🔄 Workflow Summary
1. **Data Loading & Inspection**  
   - Load CSV files for each crop/year.  
   - Label datasets (`1` for rice, `0` for cotton).  
2. **EDA**  
   - Seasonal NDVI trends, correlation analysis.  
3. **Preprocessing**  
   - Remove duplicates, handle outliers, balance classes.  
4. **Model Training**  
   - Train-test splits (80-20).  
   - Hyperparameter tuning via GridSearchCV.  
5. **Evaluation**  
   - Metrics: Accuracy, Precision, Recall, F1-Score.  
   - Clustering: Silhouette Score, NMI, Purity.  

