# 🛡️ IoT Device Profiling & Identification using Machine Learning

## 📌 Project Overview
The rapid growth of the Internet of Things (IoT) presents significant challenges in device management and security. This project addresses these challenges by developing a high-quality profiling system that identifies devices based on their unique network traffic signatures using the **CIC IoT Profiling dataset**.

---

## 📊 Detailed Dataset Insights

### 1. Source & Tools
* **Origin:** Developed by the Canadian Institute for Cybersecurity (CIC).
* **Paper Reference:** *"Towards the Development of a Realistic Multidimensional IoT Profiling Dataset"*.
* **Capture Tools:** Network packets were captured using **Wireshark** and **Dumpcap**.

### 2. Device Categorization
The dataset profiles **60 different IoT devices** from various brands across three primary protocols: **WiFi, ZigBee, and Z-Wave**. 
* **Categories:** Camera (84%), Audio (8%), and Home Automation (8%).
* **Operational Phases:** Behavior was captured during Power On, Power Off, Active, and Interactions.

### 3. Data Engineering (Final Dataset Construction)
* **Initial State:** 651 individual CSV files merged into a unified master dataset.
* **Dimensions:** **229,757 rows** and **51 features**.
* **Engineered Features:** Added `Device_Name` and `Device_Number` for categorical mapping to ensure numeric compatibility for ML training.

---

## 🛠️ Methodology & Technical Process
1. **EDA:** Conducted thorough analysis to confirm zero null values or duplicates.
2. **Preprocessing:** Dropped non-numeric features (e.g., `Device_type`) and performed feature scaling.
3. **Data Split:** 80% Training and 20% Testing set.
4. **Implementation:** Trained and compared four major ML models: Linear Regression, Perceptron, Decision Tree, and Random Forest.

---

## 📈 Performance Evaluation & Results

| Metric | Linear Regression | Perceptron | Decision Tree | Random Forest |
| :--- | :--- | :--- | :--- | :--- |
| **Test Accuracy** | 29.83% | 83.15% | 99.98% | **99.99%** |
| **MSE** | 0.1170 | 0.1684 | 0.0002 | **6.52e-05** |
| **RMSE** | 0.3420 | 0.4104 | 0.0154 | **0.0080** |

### 🔬 Technical Discussion
* **Top Performer:** **Random Forest** achieved the highest accuracy (**99.99%**) and the lowest **MSE**. Its ability to combine multiple decision trees makes it exceptionally robust for high-dimensional IoT data.
* **Underfitting:** **Linear Regression** performed poorly (29.83%) as it assumes a linear relationship, whereas IoT packet identification is inherently a non-linear classification problem.
* **Overfitting vs. Generalization:** While tree-based models showed near-perfect results, their **Zero Bias** and **negligible Variance** suggest they accurately captured the underlying patterns of network communication rather than noise.
* **Model Stability:** With a Bias of **0.1677** and Variance of **0.1684**, the Perceptron model proved less stable compared to tree-based algorithms.

---

## 📌 Conclusion
This project successfully demonstrates that network traffic patterns are highly effective for IoT device identification. By implementing **Random Forest**, we achieved near-perfect accuracy, providing a robust solution for automated network security and device profiling in smart environments.

---
**Maintained by:** Jannatul Ferdous  
**Course:** CSE303 (Data Science)  
**Tools:** Python, NumPy, Pandas, Scikit-Learn, Matplotlib, Seaborn
