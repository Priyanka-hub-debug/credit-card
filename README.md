# 💳 Credit Card Classification using Machine Learning

## 📌 Project Overview

This project focuses on building a **Machine Learning classification model for Credit Card Default Prediction**. The main objective is to predict whether a credit card customer is likely to default on their next month's payment based on customer-related financial and demographic information.

The project includes important Machine Learning steps such as **data preprocessing, exploratory data analysis, outlier handling, categorical encoding, class balancing using SMOTE, feature selection, data transformation, feature scaling, model training, prediction, and model evaluation**.

Four different Machine Learning classification algorithms were implemented and compared to identify the best-performing model.

---

## 🎯 Objectives

* Analyze and understand the credit card dataset.
* Perform data preprocessing and cleaning.
* Handle outliers using the IQR method.
* Encode categorical variables.
* Balance the target classes using SMOTE.
* Select important features using SelectKBest.
* Apply Yeo-Johnson transformation.
* Scale the selected features using StandardScaler.
* Train multiple Machine Learning classification algorithms.
* Evaluate the performance of each model.
* Compare the models using different evaluation metrics.
* Identify the best-performing classification algorithm.

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook / Anaconda**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Imbalanced-learn**

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Exploration
   ↓
Data Cleaning & Preprocessing
   ↓
Outlier Handling using IQR
   ↓
Categorical Encoding
   ↓
SMOTE Class Balancing
   ↓
Feature Selection using SelectKBest
   ↓
Yeo-Johnson Transformation
   ↓
Standard Scaling
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Model Evaluation
   ↓
Algorithm Comparison
   ↓
Best Model Selection
```

---

## 📊 Dataset

The dataset contains **30,000 records and 25 columns** before preprocessing.

Important features include:

* `LIMIT_BAL` – Amount of given credit
* `SEX` – Customer gender
* `EDUCATION` – Education level
* `MARRIAGE` – Marital status
* `AGE` – Customer age
* `PAY_0`, `PAY_2`, `PAY_3`, etc. – Repayment status
* `BILL_AMT1` to `BILL_AMT6` – Bill statement amounts
* `PAY_AMT1` to `PAY_AMT6` – Previous payment amounts
* `default payment next month` – Original target variable

The target variable was processed into a `target` column containing `NO` and `YES` classes.

---

## 🧹 Data Preprocessing

### 1. Outlier Handling

Outliers were identified and handled using an **IQR-based method** before model training.

### 2. Categorical Encoding

Categorical variables were converted into numerical representations using:

* **LabelEncoder**
* **OneHotEncoder**

### 3. Class Balancing using SMOTE

The original target classes were imbalanced.

Before applying SMOTE:

| Class |  Count |
| ----- | -----: |
| NO    | 23,364 |
| YES   |  6,636 |

**SMOTE (Synthetic Minority Over-sampling Technique)** was used to balance the target classes.

### 4. Feature Selection

**SelectKBest with f_classif** was used to select important features for classification.

### 5. Yeo-Johnson Transformation

**Yeo-Johnson Power Transformation** was applied to the numerical features to improve their distribution.

### 6. Feature Scaling

**StandardScaler** was used to standardize the selected features before model training.

### 7. Train-Test Split

The processed dataset was divided into training and testing sets using an **80:20 split** with `random_state=40`.

---

## 🤖 Machine Learning Algorithms

Four classification algorithms were used in the final project:

### 1. Logistic Regression

Logistic Regression was used as a baseline classification algorithm for predicting the target class.

### 2. Decision Tree Classifier

Decision Tree is a tree-based classification algorithm that makes predictions using feature-based decision rules.

### 3. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to improve prediction performance and reduce overfitting.

### 4. Gradient Boosting Classifier

Gradient Boosting is an ensemble Machine Learning algorithm that builds multiple models sequentially to improve classification performance.

---

## 📊 Model Evaluation

The models were evaluated using the following classification metrics:

* **Accuracy** – Measures the percentage of correctly classified observations.
* **Precision** – Measures how many predicted positive cases were actually positive.
* **Recall** – Measures how many actual positive cases were correctly identified.
* **F1-Score** – Provides a balance between precision and recall.
* **Classification Report** – Provides a detailed summary of classification performance.

---

## 📈 Model Comparison

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------: | --------: | -----: | -------: |
| Logistic Regression |      69% |       69% |    69% |      69% |
| Decision Tree       |      82% |       82% |    83% |      82% |
| Random Forest       |  **88%** |       93% |    83% |  **88%** |
| Gradient Boosting   |      87% |   **94%** |    80% |      87% |

---

## 🏆 Best Performing Model

Based on the evaluation results, **Random Forest Classifier** achieved the highest overall accuracy.

**Accuracy:** 88%
**Precision:** 93%
**Recall:** 83%
**F1-Score:** 88%

Therefore, **Random Forest Classifier** performed best overall among the four selected algorithms based on accuracy and its overall balance of evaluation metrics.

---

## 📂 Project Structure

```text
Credit-Card-Classification/
│
├── creditcard.csv
├── credit card project.ipynb
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Install Python or Anaconda

Make sure Python or Anaconda is installed on your system.

### 2. Install Required Libraries

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
```

### 3. Place the Dataset

Place `creditcard.csv` in the project directory.

### 4. Open the Jupyter Notebook

```bash
jupyter notebook
```

Open the project notebook and run the cells step by step.

---

## 📚 Key Learning Outcomes

Through this project, I gained practical knowledge of:

* Data preprocessing
* Exploratory Data Analysis
* Outlier handling
* Categorical encoding
* SMOTE class balancing
* Feature selection
* Yeo-Johnson transformation
* Feature scaling
* Classification algorithms
* Model training and prediction
* Model evaluation
* Model comparison
* Machine Learning workflow using Python

---
## ⭐ Conclusion

This project demonstrates the complete process of developing a **Machine Learning classification solution for credit card default prediction**, starting from data preprocessing and exploratory analysis to model training and evaluation.

By implementing and comparing four classification algorithms, the project provides practical experience in solving classification problems and selecting an appropriate predictive model.

Among the four models tested, **Random Forest Classifier achieved the best overall accuracy of 88%**.


