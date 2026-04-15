## 📌 Project Overview
This project performs a **comparative evaluation of multiple classification algorithms** on the Titanic dataset to predict whether a passenger survived or not.

- 📊 Dataset: Titanic (Kaggle)
- 🎯 Goal: Binary Classification (Survived / Not Survived)
- 👥 Total Samples: 1309 passengers
- 🔢 Total Features: 12

### 📂 Dataset Distribution
To ensure reliable training and evaluation, the dataset was split into training and testing sets:

- 🧠 Training Set: 891 passengers (used for model learning and pattern recognition)
- 🧪 Test Set: 418 passengers (used for evaluating performance on unseen data)

---

## 🧹 Data Preprocessing
- Missing value handling:
  - `Age`, `Fare` → filled with mean values  
  - `Embarked` → filled with most frequent value ('C')
- Removed unnecessary features:
  - `PassengerId`, `Name`, `Ticket`, `Cabin`
- Data preprocessing steps included:
  - Data cleaning  
  - Data integration  
  - Data transformation  

---

## 🔍 Feature Selection
Applied **MRMR (Minimum Redundancy Maximum Relevance)** for selecting the most important features.

### ✅ Selected Features:
- Age  
- Sex  
- Embarked  
- SibSp  
- Pclass  

---

## 📊 Data Analysis & Visualization
- 📈 Correlation heatmap analysis  
- 👩 Gender-based survival distribution  
- 🎟️ Passenger class (Pclass) survival analysis  
- 🚢 Embarkation port survival analysis  
- 🧭 Dimensionality reduction using **t-SNE** for visualization  

---

## 🤖 Machine Learning Models Used
The following classification algorithms were implemented and compared:

- Logistic Regression  
- Random Forest  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  
- AdaBoost  
- Gradient Boosting  
- Decision Tree  

---

## ⚙️ Model Evaluation Metrics
The models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

---

## 📈 Model Performance Comparison

| Algorithm            | Accuracy | Precision | Recall | F1 Score |
|---------------------|----------|-----------|--------|----------|
| Logistic Regression | 0.88     | 0.86      | 0.83   | 0.83     |
| SVM                 | 0.87     | 0.80      | 0.86   | 0.83     |
| AdaBoost            | 0.86     | 0.86      | 0.80   | 0.83     |
| Random Forest       | 0.83     | 0.79      | 0.79   | 0.79     |
| KNN                 | 0.80     | 0.80      | 0.68   | 0.74     |

---

## 🧠 Key Insights
- 👩 Female passengers had significantly higher survival rates than male passengers  
- 🎟️ First-class passengers had the highest survival probability  
- ⚓ Passengers from Cherbourg (C) showed relatively higher survival rates  
- 📌 Feature selection improved model performance and reduced complexity  

---

## 🏆 Best Performing Model
👉 **Logistic Regression achieved the highest accuracy (~88%)**

---

## 📉 Limitations
- Dataset contains missing and incomplete information  
- Class imbalance may affect model performance  
- Additional feature engineering could further improve results  

---

## ✅ Conclusion
This project demonstrates that **effective preprocessing, feature selection, and model comparison** significantly improve machine learning performance. Among all tested models, **Logistic Regression performed the best for this dataset**.
