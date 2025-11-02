# 🍷 Feature Engineering and Data Preprocessing – Wine Quality Dataset

## 📘 Overview
This project demonstrates feature engineering and data preprocessing using the **Wine Quality Dataset** from the **UCI Machine Learning Repository**.  
The goal is to prepare the dataset for regression modeling to predict the **quality score of wines** based on physicochemical properties such as acidity, pH, sugar, and alcohol content.

---

## 📂 Dataset Information
- **Dataset Name:** Wine Quality Dataset  
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/wine+quality)  
- **Type:** Regression Problem  
- **Target Variable:** `quality` (integer values between 0–10)  
- **Number of Instances:** 1,599 (Red Wine)  
- **Number of Attributes:** 12 (11 features + 1 target)

### Key Features
| Feature | Description |
| `fixed acidity` | Non-volatile acids in wine |
| `volatile acidity` | Acetic acid levels affecting taste |
| `citric acid` | Adds freshness to wine |
| `residual sugar` | Sugar remaining after fermentation |
| `chlorides` | Amount of salt in the wine |
| `free sulfur dioxide` | SO₂ in free form, prevents oxidation |
| `total sulfur dioxide` | Total SO₂ concentration |
| `density` | Wine density |
| `pH` | Acidity level |
| `sulphates` | Contributes to SO₂ levels |
| `alcohol` | Alcohol content (%) |
| `quality` | Target: wine quality score (0–10) |

---

## ⚙️ Steps Performed

1. **Data Loading & Exploration**
   - Loaded the dataset and checked for missing values, data types, and basic statistics.
   - Visualized data distribution using histograms and correlation heatmaps.

2. **Missing Value Handling**
   - Checked for NaN or null values.
   - Imputed any missing numeric values using the **mean** strategy.

3. **Encoding Categorical Variables**
   - No categorical variables exist in this dataset, but demonstrated encoding methods for completeness (e.g., LabelEncoder).

4. **Feature Scaling**
   - Standardized all numeric features using **StandardScaler** to ensure uniform contribution.

5. **Feature Extraction (PCA)**
   - Applied **Principal Component Analysis (PCA)** to reduce the dataset into fewer dimensions while retaining 95% variance.

6. **Feature Selection**
   - Used **SelectKBest (f_regression)** to identify top predictors of wine quality.

7. **Visualization**
   - Correlation heatmap to identify relationships.
   - Boxplots and scatterplots to understand outliers and variable impact.

---

## 📊 Summary of Transformations

| Step | Technique | Impact |
|------|------------|--------|
| Missing Data | Mean Imputation | No null values remain |
| Scaling | StandardScaler | Balanced numeric features |
| PCA | 2 Components | Dimensionality reduction |
| Feature Selection | SelectKBest | Identified top predictors |
| Visualization | Correlation Heatmap | Better feature understanding |

**Top Features Identified:**  
`alcohol`, `volatile acidity`, `sulphates`, `citric acid`, `density`

---

## 🧠 Observations
- **Alcohol** and **volatile acidity** are strong predictors of wine quality.  
- PCA reduced redundancy while keeping variance high.  
- The dataset became fully numeric and standardized, ready for regression modeling.

---

## ⚖️ Ethical Considerations
Although this dataset does not involve personal or demographic data, it’s still essential to:
- Ensure **no manipulation or bias** in data interpretation.
- Report preprocessing and feature selection steps transparently.
- Avoid overfitting or misrepresenting results during analysis.

---

## 🧩 Tools and Libraries Used
- Python 3  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn (PCA, StandardScaler, SelectKBest)

---

## 📁 Files in Repository

| File Name | Description |
|------------|-------------|
| `Feature_Engineering_WineQuality.ipynb` | Main Jupyter Notebook with all preprocessing steps |
| `Feature_Engineering_Report.pdf` | 1–2 page summary of the work |
| `README.md` | Documentation and ethical notes |

---

## 👨‍💻 How to Run
Click to above link https://colab.research.google.com/drive/1ca1PZ_3-RH-LpPWCzd89MPRj29dSs6rC?usp=sharing
