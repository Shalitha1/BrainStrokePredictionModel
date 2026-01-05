# 🧠 **Stroke Prediction XGBoost Model**



## 🎯 About the Project
Stroke is the **5th leading cause of death in the United States** and a major cause of long-term disability worldwide. **80% of strokes are preventable** through early identification of risk factors and appropriate interventions.  

This project develops an advanced machine learning model using **XGBoost (Extreme Gradient Boosting)** to predict stroke risk based on patient demographics, medical history, and lifestyle factors. The model serves as a **screening tool** to help healthcare providers identify high-risk patients for preventive interventions.

### 🎓 Academic Context
This project was developed as part of a healthcare machine learning course, focusing on:  
- Handling severely imbalanced medical datasets (19:1 ratio)  
- Clinical interpretability and explainable AI (SHAP analysis)  
- Real-world deployment considerations for healthcare applications  
- Comprehensive evaluation beyond simple accuracy metrics

### 🔬 Key Objectives
- Predict stroke occurrence using **11 clinical and demographic features**  
- Address class imbalance through **SMOTE** and class weight optimization  
- Provide explainable predictions using **SHAP (SHapley Additive exPlanations)**  
- Optimize for clinical relevance focusing on **recall (sensitivity)** to minimize missed diagnoses  
- Create a deployment-ready solution suitable for **primary care settings**

---

## 📊 Dataset Details
- **Dataset Name:** Brain Stroke Dataset  
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)  
- **Number of Records:** 5110 (example, replace with your dataset size)  
- **Features Include:** Age, Gender, Hypertension, Heart Disease, Marital Status, Work Type, Residence Type, Average Glucose Level, BMI, Smoking Status, etc.  
- **License:** Open Dataset (e.g., CC BY 4.0)

---

## ✨ Features / Highlights

### 🚀 Core Capabilities
- **🎯 Accurate Prediction:** 85.96% accuracy, 78.90% ROC-AUC on test data  
- **⚖️ Class Imbalance Handling:** SMOTE + XGBoost scale_pos_weight for balanced learning  
- **📊 Comprehensive EDA:** 15+ visualizations analyzing data distributions and correlations  
- **🔍 Feature Importance:** Identifies top risk factors (age, work type, glucose, BMI)  
- **🧠 Explainable AI:** SHAP analysis for transparent, interpretable predictions  
- **📈 Hyperparameter Optimization:** RandomizedSearchCV with 50 iterations, 5-fold CV  
- **🩺 Clinical Focus:** Emphasizes recall (34%) to reduce missed stroke diagnoses  
- **💾 Reproducible Pipeline:** Fixed random seeds, documented preprocessing steps  
- **📉 Error Analysis:** Detailed false positive/negative analysis with clinical interpretation  
- **🖥️ Resource Efficient:** Runs on standard laptops (8GB RAM, no GPU required)  

### 📋 Technical Highlights
- Advanced Preprocessing: Missing value imputation, outlier analysis, feature scaling  
- Multiple Encoding Strategies: Label encoding (binary) + One-hot encoding (multi-class)  
- Model Validation: Stratified train/validation/test split (64%/16%/20%)  
- Performance Tracking: Training curves, loss monitoring, convergence analysis  
- Multiple Metrics: Accuracy, Precision, Recall, F1, ROC-AUC, Confusion Matrix  
- Visualization Suite: 20+ publication-quality plots for analysis and reporting  

---

## 🛠️ Installation / How to Run

### Prerequisites
- Python 3.8 or higher  
- pip package manager  
- 8GB RAM minimum (16GB recommended)  
- Operating System: Windows, macOS, or Linux  

### 📥 Quick Start

1️⃣ **Clone the Repository**  
```bash
git clone https://github.com/yourusername/stroke-prediction-xgboost.git
cd stroke-prediction-xgboost

### Install Dependencies
pip install -r requirements.txt

