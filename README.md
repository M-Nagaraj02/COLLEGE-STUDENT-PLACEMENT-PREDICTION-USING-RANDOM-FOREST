---
# 🎓 College Student Placement Prediction using Random Forest
---
## 📌 Overview

This project focuses on predicting whether a college student will get placed or not using Machine Learning classification techniques.

The primary algorithm used in this project is:

* 🌲 Random Forest Classifier

The model is trained on academic and performance-related features to predict student placement status with high accuracy.

---

## 📊 Dataset Information

Total Records: 10,000
Total Features: 8 input features
Target Variable: Placement (0 = Not Placed, 1 = Placed)

**Target:**

Placement

---

##🛠️ Libraries 
``` python
import pandas as pd
import numpy as np
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.metrics import confusion_matrix
```
---

## 🧹 Data Preprocessing

**✅ Data Cleaning**

* No Missing Values
* No Duplicate Values
  
Categorical Columns Converted:

* Internship_Experience → Yes/No → 1/0
* Placement → Yes/No → 1/0

**📊 Dataset Shape**
```
(10000, 10)
```
**📌 Class Distribution**

* Not Placed (0) → 8341
* Placed (1) → 1659

## 🔀 Train-Test Split

* 80% Training Data
* 20% Testing Data
* random_state = 2

---

## 🌲 Random Forest Model

Model Used:
```python
RandomForestClassifier(n_estimators=100, random_state=42)
```
---
## 📈 Model Performance

**✅ Accuracy Score**
* Accuracy: 0.9995
## 📊 Confusion Matrix
```
[[1667    0]
 [   1  332]]
```
---

## 📄 Classification Report
```
Class	           Precision	Recall	F1-Score
Not Placed (0)      	1.00	 1.00	   1.00
Placed (1)          	1.00	 1.00	   1.00
```
**🎯 Key Insight**

The Random Forest model achieved near-perfect classification performance on test data.

## 📊 Visualization

**Confusion Matrix visualized using heatmap with:**

* seaborn
* matplotlib

<img width="658" height="547" alt="image" src="https://github.com/user-attachments/assets/37950a71-ceac-49cd-8e3b-55a4cfbda8ae" />

**Heatmap helps visually understand:**

* True Positives
* True Negatives
* False Positives
* False Negatives

---

## 📂 Project Structure
```
Student-Placement-Prediction/
│── placement_prediction.ipynb
│── college_student_placement_dataset.csv
│── README.md
```
---

## 👨‍💻 Author

**Nagaraj M**

GitHub: https://github.com/M-Nagaraj02
