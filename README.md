# 🛡️ Sprint 14 Project — Insurance Benefits Prediction & Data Masking with Linear Algebra

---

## 🧠 Project Overview

In this project, I worked with **Sure Tomorrow Insurance**, a company interested in applying machine learning and linear algebra techniques to solve several business problems related to customer analysis, insurance benefit prediction, and data privacy.

The project combines practical machine learning applications with fundamental linear algebra concepts, demonstrating how mathematical transformations can protect sensitive customer information without affecting model performance.

Four independent tasks were completed:

1. Customer similarity analysis.
2. Insurance benefit classification.
3. Insurance benefit quantity prediction.
4. Data masking and privacy protection.

---

## 🎯 Project Objectives

* Explore and validate customer insurance data.
* Identify customers similar to a given customer.
* Predict whether a customer will receive insurance benefits.
* Predict the number of insurance benefits a customer may receive.
* Compare machine learning models against baseline (dummy) models.
* Develop a data masking algorithm using linear algebra.
* Demonstrate that data protection does not reduce model quality.

---

## 📁 Dataset Description

**File:** `insurance_us.csv`

The dataset contains demographic and financial information about insured individuals.

### Features

| Column         | Description              |
| -------------- | ------------------------ |
| Gender         | Customer gender          |
| Age            | Customer age             |
| Salary         | Annual salary            |
| Family Members | Number of family members |

### Target Variable

| Column             | Description                                                      |
| ------------------ | ---------------------------------------------------------------- |
| Insurance Benefits | Number of insurance benefits received during the last five years |

---

## 🧩 Project Workflow

### Step 1 — Data Preparation

* Loaded and inspected the dataset.
* Verified data types.
* Checked for missing values.
* Investigated duplicate records.
* Examined distributions and potential outliers.
* Prepared the dataset for machine learning tasks.

---

## 🔍 Task 1 — Customer Similarity Analysis

The first objective was to identify customers who are most similar to a selected individual.

### Methodology

* Applied distance-based similarity measures.
* Implemented the k-Nearest Neighbors (kNN) algorithm.
* Compared customer similarity using different scaling approaches.

### Key Questions

* How does feature scaling affect nearest-neighbor selection?
* Which customers are most similar to a given individual?

### Outcome

The analysis demonstrated that feature scaling significantly impacts similarity calculations and improves the quality of nearest-neighbor searches.

---

## 🤖 Task 2 — Insurance Benefit Classification

The second objective was to predict whether a customer would receive at least one insurance benefit.

### Approach

A binary classification problem was created:

```text
0 = No Insurance Benefits
1 = Received Insurance Benefits
```

### Models Evaluated

* Dummy Classifier (Baseline)
* k-Nearest Neighbors Classifier

### Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score

### Outcome

The trained machine learning model was compared against a baseline model to determine whether predictive learning provided meaningful improvements.

---

## 📈 Task 3 — Insurance Benefit Prediction

The third objective was to estimate the number of insurance benefits a customer might receive.

### Model Used

* Linear Regression

### Evaluation Metrics

* RMSE (Root Mean Squared Error)
* R² Score

### Outcome

The regression model successfully estimated expected insurance benefits based on customer characteristics.

---

## 🔒 Task 4 — Data Masking Using Linear Algebra

The final objective was to protect sensitive customer information without reducing model performance.

### Methodology

A data transformation approach based on matrix multiplication was implemented.

Steps:

1. Create a random invertible matrix.
2. Transform the original feature matrix.
3. Train the regression model using transformed data.
4. Compare model performance before and after transformation.

### Mathematical Concept

The transformation follows:

```text
X' = X × P
```

Where:

* X = Original feature matrix
* P = Invertible transformation matrix
* X' = Masked dataset

---

## 📊 Data Privacy Validation

The project demonstrates that:

* Personal information becomes difficult to reconstruct.
* Sensitive customer data remains protected.
* Machine learning model quality remains unchanged.

Theoretical proof and empirical validation were performed to confirm that linear regression predictions are preserved after transformation.

---

## 📚 Linear Algebra Concepts Applied

* Matrix Multiplication
* Matrix Inversion
* Linear Transformations
* Vector Representation
* Euclidean Distance
* Feature Space Transformation

---

## 📊 Evaluation Metrics

### Classification

* Accuracy
* Precision
* Recall
* F1-Score

### Regression

* RMSE
* R² Score

### Similarity Search

* Euclidean Distance
* k-Nearest Neighbors

---

## 💡 Business Insights

This project illustrates how machine learning can support insurance companies by:

* Identifying similar customer profiles.
* Predicting benefit eligibility.
* Forecasting expected claim activity.
* Protecting sensitive customer information.
* Maintaining regulatory compliance while preserving analytical value.

The combination of predictive modeling and data masking techniques enables organizations to balance business intelligence with privacy protection.

---

## 🧰 Tools & Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* Linear Algebra Methods
* Jupyter Notebook

---

## 📚 Machine Learning Concepts Applied

* k-Nearest Neighbors (kNN)
* Classification
* Regression
* Linear Regression
* Feature Scaling
* Model Evaluation
* Data Privacy
* Data Masking
* Matrix Transformations
* Applied Linear Algebra

---

## 👤 Author

**Jonathan Peña**
