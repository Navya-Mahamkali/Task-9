# Task-9
# Credit Card Fraud Detection using Machine Learning

## 📌 Overview
This project aims to detect fraudulent transactions using machine learning techniques. Due to the highly imbalanced nature of fraud datasets, special attention is given to evaluation metrics such as precision, recall, and F1-score instead of accuracy.

---

## 📂 Dataset Information
- Dataset: Credit Card Fraud Detection Dataset
- Target Variable:
  - Class (0 = Non-Fraud, 1 = Fraud)

### Key Features:
- V1 to V28 (anonymized features)
- Amount
- Time (optional)

---

## ⚙️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Joblib

---

## 🔧 Project Workflow

### 1. Data Loading & Exploration
- Loaded dataset using Pandas
- Checked class imbalance using value counts and visualization

### 2. Data Preprocessing
- Removed non-useful columns (if any)
- Separated features (X) and target (y)

### 3. Train-Test Split
- Used stratified sampling to preserve fraud ratio
- 80% training and 20% testing

### 4. Baseline Model
- Logistic Regression used as a baseline model
- Applied StandardScaler for feature scaling

### 5. Advanced Model
- Random Forest Classifier with:
  - n_estimators = 100
  - random_state = 42

### 6. Model Evaluation
- Evaluated using:
  - Precision
  - Recall
  - F1-score
- Accuracy avoided due to imbalance

### 7. Feature Importance
- Extracted and visualized top contributing features using Random Forest

### 8. Model Comparison
- Compared Logistic Regression vs Random Forest using F1-score

### 9. Model Saving
- Best model saved using Joblib for future use

---

## 📊 Results
- Random Forest outperformed Logistic Regression in detecting fraud cases
- High recall achieved for fraud class, which is critical in real-world scenarios

---

## 📈 Outputs
- Class imbalance plot
- Classification reports
- Feature importance graph
- Saved model file (.pkl)

---

## 🎯 Key Learnings
- Handling imbalanced datasets
- Importance of recall in fraud detection
- Comparing baseline and advanced models
- Feature importance interpretation

---

## 🚀 Future Improvements
- Apply SMOTE for balancing data
- Hyperparameter tuning
- Use advanced models like XGBoost
- Deploy model using Flask/Streamlit

---

## 👩‍💻 Author
Navya Mahamkali
