# credit-card-fraud-detection
End-to-end machine learning project for fraud detection
# 💳 Credit Card Fraud Detection (End-to-End Machine Learning Project)

## 📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques.

The dataset is highly imbalanced:
- Normal transactions: 99.83%
- Fraud transactions: 0.17%

Because of this imbalance, accuracy alone is not a reliable metric. Instead, Precision, Recall, F1-score, and ROC-AUC are used for evaluation.

---

## 🎯 Objective

The main goal is to build a model that can:

- Detect fraudulent transactions accurately
- Reduce false negatives (missed frauds)
- Maintain a balance between precision and recall

---

## 📊 Dataset Information

- Type: Credit card transactions
- Target variable: Class
  - 0 → Normal transaction
  - 1 → Fraudulent transaction
- Strong class imbalance problem

---

## 🧠 Techniques Used

### 🔍 Data Analysis
- Exploratory Data Analysis (EDA)
- Class distribution visualization

### ⚙️ Data Preprocessing
- Train-test split (stratified sampling)
- Handling missing imbalance issues

### ⚖️ Imbalance Handling
- SMOTE (Synthetic Minority Oversampling Technique)
- Class weighting (scale_pos_weight)

### 🤖 Machine Learning Models
- Logistic Regression (baseline model)
- XGBoost Classifier (final model)

### 📈 Optimization Techniques
- Probability-based predictions (predict_proba)
- Threshold tuning
- Precision–Recall trade-off analysis

---

## 🚀 Model Performance

### 🏆 Final Model: XGBoost

- Precision (Fraud): 0.74  
- Recall (Fraud): 0.87  
- F1-score (Fraud): 0.80  

- Accuracy: ~1.00 (not used as main metric due to imbalance)

---

## 📉 Key Insights

- Dataset is extremely imbalanced
- Accuracy is misleading for this problem
- Logistic Regression underperformed on minority class
- XGBoost significantly improved detection performance
- Threshold tuning improved real-world usability

---

## 🎯 Threshold Optimization

Instead of using default 0.5 threshold, probability outputs were optimized to:

- Improve fraud detection (recall)
- Control false positives (precision)
- Achieve better F1-score balance

---

## 📊 Evaluation Metrics

- Confusion Matrix
- Precision / Recall / F1-score
- ROC-AUC Score
- Precision–Recall Curve
- Threshold vs F1-score analysis

---

## 🧪 Future Improvements

- Feature importance analysis (XGBoost interpretation)
- SHAP explainability
- Cost-sensitive learning (financial impact optimization)
- Advanced anomaly detection models

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

---

## 📌 Conclusion

This project demonstrates an end-to-end machine learning pipeline for fraud detection including:

- Data preprocessing
- Handling imbalanced datasets
- Model training and evaluation
- Threshold optimization

The final model is optimized not only for accuracy but also for real-world business performance.

---

## ⭐ Author

Data science learning project focused on real-world fraud detection systems.
