# Bank Marketing Campaign Prediction

## 📌 Objective
The objective of this project is to predict whether a customer will subscribe to a term deposit (`y`) using historical marketing campaign data from a Portuguese bank. The project involves data preprocessing, visualization, feature engineering, model building, and evaluation.

---

## 📊 Dataset Used

- **Name**: Bank Marketing Dataset  
- **Source**: UCI Machine Learning Repository  
- **Link**: [https://archive.ics.uci.edu/ml/datasets/Bank+Marketing](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)

- **Total Instances**: ~45,000 (after cleaning)
- **Features**: Age, Job, Marital Status, Education, Balance, Day, Duration, Campaign, Pdays, Previous, etc.
- **Target Variable**: `y` (binary classification: `yes` or `no`)

---

## 🧠 Models Used

1. **Logistic Regression**  
   - Used as a baseline model for classification.
2. **Decision Tree**  
   - Simple and interpretable; good for capturing non-linear patterns.
3. **Support Vector Machine (SVM)**  
   - Effective for high-dimensional data and clear decision boundaries.
4. **K-Nearest Neighbors (KNN)**  
   - Non-parametric, instance-based model that performs well with balanced data.
5. **Random Forest Classifier** ✅ *(Best Performer)*  
   - Ensemble model that reduces overfitting and provides feature importance.



## 🧪 Key Results

| Model                | Accuracy | F1 Score | AUC    |
|---------------------|----------|----------|--------|
| Logistic Regression | 0.88     | 0.66     | 0.84   |
| Decision Tree       | 0.89     | 0.69     | 0.85   |
| SVM                 | 0.88     | 0.66     | 0.84   |
| KNN                 | 0.87     | 0.64     | 0.83   |
| **Random Forest**   | **0.94** | **0.97** | **0.86** ✅ |
### ✅ **Best Model**: Random Forest  
- Tuned with `RandomizedSearchCV`  
- Final accuracy: **94%**, AUC: **0.86**

---

## 🔍 Highlights

- **Class Imbalance** checked and acknowledged; may benefit from resampling in future.
- **Skewness** handled using **Yeo-Johnson** transformation.
- **Outliers** removed using **IQR** and **Z-Score** methods.
- **Feature Selection** using `SelectKBest` .
- **ROC Curve** generated for best model (AUC = 0.86).
- Final model saved as `final_model.pkl`.


## 📂 Repository Contents

- `final_project.ipynb` – Full project notebook with EDA, preprocessing, modeling, and evaluation.
- `cleaned_bank_data.csv` – Final cleaned dataset used for training.
- `final_model.pkl` – Saved best model (Random Forest) using `joblib`.
- `README.md` – Project documentation file.

---

## ✅ Future Work

- Experiment with neural networks (MLP) or deep learning frameworks.
- Integrate additional data sources for feature enrichment.
- Build and deploy a prediction API or dashboard interface.

---
