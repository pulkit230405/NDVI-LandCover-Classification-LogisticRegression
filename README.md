# NDVI-LandCover-Classification-LogisticRegression
# 🌱 NDVI Land Cover Classification using Logistic Regression

This repository contains a solution to a **multiclass land cover classification** problem using **Logistic Regression**, as part of the **Summer Analytics Mid Hackathon**. The goal is to classify satellite imagery pixels based on their **NDVI (Normalized Difference Vegetation Index)** time-series patterns.

---

## 📌 Problem Statement

Given 27 NDVI readings over time for each pixel, predict the **land cover class**:

- **Water**
- **Impervious**
- **Farm**
- **Forest**
- **Grass**
- **Orchard**

### Challenges:
- Noisy satellite data due to clouds
- Missing NDVI values
- Seasonal variation in vegetation
- Model is limited to **Logistic Regression only**

---

## 🧠 Solution Overview

The solution is built using:
- 🧹 **KNN Imputation** to fill missing values
- 🧪 **Feature Engineering** on NDVI series:
  - Mean, Standard Deviation, Min, Max, Range
  - Trend (mean of 1st differences)
- ⚙️ **Standard Scaling** for normalization
- 📈 **Multiclass Logistic Regression** (`lbfgs` solver)

---

## 📁 Dataset

- `hacktrain.csv`: Training data with `ID`, 27 NDVI values, and `class`
- `hacktest.csv`: Test data with `ID` and 27 NDVI values (no class)

---

## 📦 Libraries Used

python
pandas, numpy, sklearn

🛠️ How to Run
Clone the repo:
git clone https://github.com/yourusername/NDVI-LandCover-Classification-LogisticRegression.git
cd NDVI-LandCover-Classification-LogisticRegression

Install dependencies (optional):
pip install pandas scikit-learn numpy

Run the notebook or Python script:
For Jupyter Notebook: Open ndvi_land_cover.ipynb

For script: Run python ndvi_land_cover.py

📌 Author
Pulkit Jain
GitHub: @pulkit230405

📃 License
This project is licensed under the MIT License - see the LICENSE file for details.

