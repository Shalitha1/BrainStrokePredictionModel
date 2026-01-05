# 🧠 Stroke Prediction: Advanced XGBoost Analysis

## 🎯 Project Overview
Stroke is the 5th leading cause of death and a major contributor to long-term disability worldwide. Studies indicate that **80% of strokes are preventable** through early risk identification and intervention.  

This project implements an **end-to-end machine learning pipeline using XGBoost** to predict stroke risk. Leveraging patient demographics, medical history, and lifestyle factors, the model acts as a clinical screening tool. It prioritizes **Recall (Sensitivity)** to ensure high-risk patients are not overlooked.

---

## 🔬 Key Objectives
- **Predictive Modeling:** Utilize 11 clinical features to forecast stroke occurrence.
- **Imbalance Management:** Handle the 19:1 class imbalance using **SMOTE** and `scale_pos_weight`.
- **Explainable AI (XAI):** Apply **SHAP analysis** for transparent, interpretable predictions.
- **Clinical Optimization:** Focus on minimizing **False Negatives** to support primary care decisions.

---

## 📊 Dataset & Features
The model is trained on the **Brain Stroke Dataset**.

| Feature Category | Variables |
|-----------------|-----------|
| **Demographics** | Age, Gender, Residence Type, Marital Status |
| **Clinical Metrics** | BMI, Average Glucose Level, Hypertension, Heart Disease |
| **Lifestyle** | Work Type, Smoking Status |
| **Target** | Stroke (1: Yes, 0: No) |

---

## ✨ Technical Highlights

### 🚀 Performance Metrics
- **Accuracy:** 85.96%  
- **ROC-AUC:** 78.90%  
- **Clinical Focus:** Optimized for high **Recall (34% on minority class)** to reduce missed diagnoses.  
- **Optimization:** Hyperparameter tuning via `RandomizedSearchCV` (50 iterations, 5-fold CV).

### 🛠️ Data Pipeline
- **Preprocessing:** Missing value imputation and outlier detection.
- **Encoding:** Label encoding for binary features; One-hot encoding for multi-class variables.
- **Resampling:** SMOTE to balance class distribution.
- **Analysis:** 20+ publication-quality visualizations using **Seaborn** and **Matplotlib**.

---

## 🛠️ Tech & License

**Required Packages**
- pandas>=1.5.0
- numpy>=1.23.0
- matplotlib>=3.6.0
- seaborn>=0.12.0
- scikit-learn>=1.3.0
- xgboost>=2.0.0
- imbalanced-learn>=0.11.0
- shap>=0.42.0


**Technology Stack**

| Component            | Technology                  |
|---------------------|----------------------------|
| **Language**         | Python                     |
| **Data Manipulation**| Pandas, NumPy              |
| **Machine Learning** | XGBoost, Scikit-learn      |
| **Imbalance Handling**| Imbalanced-learn (SMOTE)  |
| **Explainability**   | SHAP                       |
| **Visualization**    | Matplotlib, Seaborn        |

**License**  
This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.



