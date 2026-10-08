# Telco Customer Churn Prediction

## Project Overview

This project focuses on predicting whether a telecom customer is likely to **churn (leave the service)** using machine learning classification techniques.

The project follows a complete machine learning workflow, including **data analysis, preprocessing, exploratory data analysis (EDA), model building, and model evaluation**.

Six different classification algorithms were trained and compared to identify a suitable model for predicting customer churn.

---

## Dataset

The dataset contains information about **7,043 telecom customers**.

* **Records:** 7,043
* **Features:** 21
* **Churned Customers:** 1,869
* **Missing Values:** 0
* **Duplicate Records:** 0
* **Target Variable:** `Churn`

The target variable indicates whether a customer has left the telecom service.

---

## Project Objectives

* Understand the characteristics of telecom customers.
* Explore factors related to customer churn.
* Preprocess categorical and numerical data.
* Build multiple classification models.
* Compare model performance using different evaluation metrics.
* Select a suitable model for customer churn prediction.

---

## Exploratory Data Analysis

The dataset was explored to identify important patterns and relationships related to customer churn.

Some of the key observations include:

* Churned customers had a considerably lower average tenure than customers who stayed.
* Customer contract type showed noticeable differences in churn.
* Electronic check users showed comparatively higher churn.
* Support-related services showed differences between churned and retained customers.

These observations helped understand which customer characteristics may be associated with churn.

---

## Data Preprocessing

The following preprocessing steps were performed:

1. Checked the dataset structure and data types.
2. Checked for missing values.
3. Checked for duplicate records.
4. Converted categorical variables using **One-Hot Encoding**.
5. Standardized numerical features where required.
6. Split the dataset into training and testing sets.

### Train-Test Split

The dataset was divided into:

* **80% Training Data**
* **20% Testing Data**

---

## Machine Learning Models

Six classification algorithms were implemented and compared:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Decision Tree
4. Random Forest
5. Naive Bayes
6. Support Vector Machine (SVM)

---

## Model Evaluation

The models were evaluated using:

* Accuracy
* Precision
* Recall
* ROC-AUC

### Results

| Model                   |   Accuracy | Precision |     Recall |    ROC-AUC |
| ----------------------- | ---------: | --------: | ---------: | ---------: |
| **Logistic Regression** | **82.04%** |    68.52% |     59.52% |     0.8620 |
| KNN                     |     80.91% |    67.22% |     54.42% |     0.8413 |
| Decision Tree           |     70.83% |    44.95% |     45.31% |     0.6283 |
| Random Forest           |     81.55% |    70.40% |     52.28% | **0.8624** |
| Naive Bayes             |     66.57% |    43.59% | **89.28%** |     0.8377 |
| SVM                     |     81.41% |    69.34% |     53.35% |     0.8231 |

---

## Best Model

Based on the model comparison, **Logistic Regression** achieved the highest accuracy at **82.04%** and was selected as the preferred model in this project.

It also achieved a strong **ROC-AUC score of 0.8620**.

An important observation is that **Naive Bayes achieved the highest recall (89.28%)**, meaning it was able to identify a larger proportion of actual churned customers, although its overall accuracy was lower.

Random Forest achieved a slightly higher ROC-AUC of **0.8624**, but Logistic Regression provided the highest accuracy.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Machine Learning Workflow

```text
Dataset
   ↓
Data Understanding
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Data Preprocessing
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Best Model Selection
```

---

## Project Structure

```text
Telco_Customer_Churn_Prediction/
│
├── project_Classification.ipynb
├── README.md
└── dataset/
    └── telco_customer_churn.csv
```

---

## Key Learnings

Through this project, I gained practical experience in:

* Exploratory Data Analysis
* Handling categorical and numerical data
* One-Hot Encoding
* Feature standardization
* Classification algorithms
* Model comparison
* Accuracy, Precision, Recall and ROC-AUC
* Understanding customer churn patterns
* Building an end-to-end machine learning workflow

---

## Conclusion

This project demonstrates how machine learning classification techniques can be used to analyze and predict customer churn.

After comparing six classification algorithms, **Logistic Regression achieved the highest accuracy of 82.04%**, while **Naive Bayes achieved the highest recall of 89.28%**.

The project helped demonstrate the complete process of developing a classification model, from understanding and analyzing the dataset to preprocessing, model training, evaluation, and comparison.

---

## Disclaimer

This project is developed for **learning and portfolio purposes**. The model results should not be considered as a production-ready churn prediction system without further validation, feature engineering, and testing on real-world data.
