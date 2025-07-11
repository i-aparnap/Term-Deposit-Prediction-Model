# 📘 README.md

## 🏷️ Project Title
Bank Marketing Campaign Prediction

## 🎯 Objective
To predict whether a client will subscribe to a term deposit based on their demographic and campaign-related data using classification models.

## 📂 Dataset Used
- **Name:** Bank Marketing Dataset  
- **Source:** UCI Machine Learning Repository  
- **Link:** [https://archive.ics.uci.edu/ml/datasets/bank+marketing](https://archive.ics.uci.edu/ml/datasets/bank+marketing)

## ⚙️ Models Used
We applied and evaluated multiple machine learning models:

- **Logistic Regression**: A simple linear model used as a baseline classifier.
- **K-Nearest Neighbors (KNN)**: Captures patterns based on feature proximity.
- **Support Vector Machine (SVM)**: Used for its robustness in high-dimensional spaces.
- **Decision Tree**: Provides interpretability with rule-based predictions.
- **Random Forest**: An ensemble method that mitigates overfitting and increases performance.

These models were selected to compare linear, non-linear, and ensemble-based learning approaches for classification.

## 📊 Key Results
| Model               | Accuracy | Precision | Recall | F1 Score | AUC   |
|--------------------|----------|-----------|--------|----------|--------|
| Logistic Regression| 0.8929   | 0.2483    | 0.4537 | 0.3209   | 0.8202 |
| KNN                | 0.9004   | 0.2349    | 0.3482 | 0.2806   | 0.7659 |
| SVM                | 0.9304   | 0.3904    | 0.4441 | 0.4155   | 0.8760 |
| Decision Tree      | 0.9002   | 0.2515    | 0.3994 | 0.3086   | 0.6646 |
| Random Forest      | 0.9403   | 0.4491    | 0.3099 | 0.3667   | 0.9056 |

- 📌 **Best Performing Model:** **Random Forest** with highest accuracy and AUC score.

## 📈 Interpretation of Results (Conclusion)
- Random Forest outperformed all other models in terms of accuracy and AUC, indicating better generalization.
- However, all models struggled with low recall on the minority class due to class imbalance.
- The dataset was heavily skewed (imbalance ratio ~17:1), which influenced the ability to predict the "yes" class effectively.
- Feature scaling, outlier handling, and transformation (Yeo-Johnson) helped improve model performance and interpretability.

## 🚀 Future Work
To enhance the model’s robustness and practical use:

1. **🔍 Explore Deep Learning Techniques:**
   - Use neural networks to capture deeper patterns in data.

2. **📈 Periodic Model Updates:**
   - Retrain with new data to address concept drift.

3. **⚖️ Improve Class Balance Techniques:**
   - Experiment with hybrid resampling methods like SMOTE-ENN.

4. **🧠 Feature Engineering Enhancements:**
   - Derive features like contact frequency, campaign efficiency, or time-based patterns.

5. **📊 Real-Time Deployment:**
   - Monitor live performance using dashboards and alerts.

6. **🧪 Ensemble Stacking:**
   - Combine multiple models to boost performance.

---
