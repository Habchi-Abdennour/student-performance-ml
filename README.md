# Student Performance Prediction (Multiple Linear Regression)

This project is a beginner-friendly machine learning exercise based on a Kaggle dataset.  
The goal is to predict the **Performance Index** of students using multiple academic and lifestyle features.

---

## Dataset

The dataset contains **10,000 rows** and the following columns:

- **Hours Studied** (int)  
- **Previous Scores** (int)  
- **Extracurricular Activities** (Yes / No)  
- **Sleep Hours** (int)  
- **Sample Question Papers Practiced** (int)  
- **Performance Index** (float) → target variable  

Source: Kaggle (Student Performance dataset)

---

## Preprocessing Steps

1. **Binary Encoding**
   - Converted `Extracurricular Activities` from `Yes / No` to `1 / 0`.

2. **Train / Test Split**
   - 70% training data
   - 30% testing data
   - `random_state = 42`

3. **Feature Scaling**
   - Applied `StandardScaler` to numeric features:
     - Hours Studied
     - Previous Scores
     - Sleep Hours
     - Sample Question Papers Practiced
   - Binary column was left unchanged.

---

## Model

- **Multiple Linear Regression**
- Implemented using `scikit-learn`

---

## Evaluation Metrics

The model was evaluated on the test set using:

- **R² Score** ≈ 0.99 
- **Mean Squared Error (MSE)** ≈ 4.08  
- **Mean Absolute Error (MAE)** ≈ 1.61 


These results indicate that the model explains most of the variance in the target variable.

---

## Residual Analysis

Residuals were computed as:

Residual = Actual Value − Predicted Value


A histogram of residuals was plotted to evaluate model assumptions:

- Residuals are centered around 0
- Distribution is approximately normal
- No strong skewness or extreme outliers

This suggests that linear regression is an appropriate model for this dataset.

---

## Tools & Libraries

- Python
- pandas
- seaborn
- scikit-learn

---

## Purpose

This project is for **learning and practice**, focusing on:
- Proper preprocessing
- Avoiding data leakage
- Model evaluation
- Basic diagnostic analysis (residuals)

---


=======
# student-performance-ml
End-to-end machine learning project using multiple linear regression to predict student performance. Includes data preprocessing, feature scaling, model evaluation, and residual analysis using a Kaggle dataset.
