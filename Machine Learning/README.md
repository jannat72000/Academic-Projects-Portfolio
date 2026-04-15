## 📌 Project Overview
This project performs a **comparative evaluation of multiple classification algorithms** on the Titanic dataset to predict whether a passenger survived or not.

- 📊 Dataset: Titanic (Kaggle)
- 🎯 Goal: Binary Classification (Survived / Not Survived)
- 👥 Total Samples: 1309 passengers
- 🔢 Total Features: 12

---

## 🧹 Data Preprocessing
- Missing value handling:
  - `Age`, `Fare` → filled with mean
  - `Embarked` → filled with 'C'
- Removed unnecessary columns:
  - `PassengerId`, `Name`, `Ticket`, `Cabin`
- Steps performed:
  - Data Cleaning  
  - Data Integration  
  - Data Transformation  

---

## 🔍 Feature Selection
Used **MRMR (Minimum Redundancy Maximum Relevance)** to select the most important features.

### ✅ Selected Features:
- Age  
- Sex  
- Embarked  
- SibSp  
- Pclass  

---

## 📊 Data Analysis & Visualization
- 📈 Correlation Heatmap
- 👩‍🦰 Gender-based survival analysis
- 🎟️ Passenger class analysis
- 🚢 Embarkation port analysis
- 🧭 t-SNE used for dimensionality reduction & visualization

---

## 🤖 Machine Learning Models Used
- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  
- AdaBoost  
- Gradient Boosting  
- Decision Tree  

---

## ⚙️ Model Evaluation Metrics
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

## 📈 Model Performance

| Algorithm           | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|----------|--------|----------|
| Logistic Regression| 0.88     | 0.86     | 0.83   | 0.83     |
| SVM                | 0.87     | 0.80     | 0.86   | 0.83     |
| AdaBoost           | 0.86     | 0.86     | 0.80   | 0.83     |
| Random Forest      | 0.83     | 0.79     | 0.79   | 0.79     |
| KNN                | 0.80     | 0.80     | 0.68   | 0.74     |

---

## 🧠 Key Insights
- 👩 Female passengers had significantly higher survival rates than males
- 🎟️ 1st class passengers had the highest survival probability
- ⚓ Passengers from Cherbourg (C) showed better survival rates
- 📌 Feature selection improved model performance and reduced complexity

---

## 🏆 Best Model
👉 **Logistic Regression achieved the highest accuracy (~88%)**

---

## 📉 Limitations
- Dataset contains missing and limited features
- Class imbalance may affect performance
- More feature engineering could improve results

---

## ✅ Conclusion
This project shows that **proper data preprocessing, feature selection, and model comparison** are crucial for improving machine learning performance. Among all models, **Logistic Regression performed best for this dataset**.

