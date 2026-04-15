## 📌 Project Overview
This project was developed for the **Artificial Intelligence** course. The goal is to predict the survival probability of Titanic passengers based on attributes such as age, gender, and ticket class using classic Machine Learning algorithms.

## 📊 Dataset Insights
* **Source:** Collected from Kaggle.
* **Size:** 418 rows and 12 columns (Testing set) and 891 rows (Training set).
* **Target Variable:** `Survived` (0 = No, 1 = Yes).
* **Key Features:** Pclass, Gender, Age, Fare, and Embarked.

### Data Preprocessing
* **Missing Values:** Imputed missing 'Age' values using the **Median** and missing 'Fare' values using the **Mode**.
* **Feature Engineering:** Dropped non-contributing columns like `PassengerId`, `Name`, `Ticket`, and `Cabin` to reduce dimensionality.
* **Correlations:** Performed Heatmap analysis to identify relationships between features and survival odds.

## 🛠️ Methodology & Implementation
We compared two fundamental AI approaches for binary classification:

### 1. Naive Bayesian Classifier
* A generative learning model based on **Bayes' Theorem**.
* Used the **Probability Density Function (PDF)** for continuous features (Age, Fare).
* Calculated likelihood for discrete features (Gender, Pclass, Embarked).

### 2. Single Layer Perceptron (SLP)
* A threshold-based artificial neural network.
* Implemented training over multiple epochs to optimize weights using **NumPy**.
* Focused on finding a linear decision boundary for binary classification.

## 📈 Performance Results
| Algorithm | Test Accuracy | Observations |
| :--- | :--- | :--- |
| **Naive Bayesian** | **100.00%** | Exceptional precision with categorical and continuous features. |
| **Single Layer Perceptron** | **58.73%** | Lower accuracy suggests the data might not be perfectly linearly separable. |

## 🧪 Key Findings & Conclusion
* **Naive Bayes** proved to be the superior model for this specific dataset due to its efficiency with independent features.
* The **Perceptron** model's performance highlights the complexity of the dataset, suggesting that future improvements could include deep neural networks or more advanced feature engineering.

