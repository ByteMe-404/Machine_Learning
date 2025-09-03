# 📏 Feature Scaling

**Feature Scaling** is the process of bringing all numeric features to the same scale (range or distribution).  
Many Machine Learning algorithms are sensitive to differences in magnitude — a column measured in kilometers may dominate one measured in centimeters.  

---

## 🔹 Why Feature Scaling?
- Ensures **fair comparison** between features.  
- Makes **gradient descent converge faster** (used in Linear Regression, Logistic Regression, Neural Networks).  
- Required for **distance-based algorithms** (KNN, K-Means, PCA, SVM).  
- Not always needed for **tree-based models** (Decision Trees, Random Forest, XGBoost).  

---

## 🔹 Common Methods

## 1. Min-Max Normalization

**Formula:**

X_norm = (X - X_min) / (X_max - X_min)


| Symbol           | Meaning                                              |
|-----------------|------------------------------------------------------|
| X               | Original value of a feature                          |
| X_min           | Minimum value of the feature in the dataset         |
| X_max           | Maximum value of the feature in the dataset         |
| X_norm          | Normalized value scaled to [0,1]                    |

**Explanation:**  
- Subtract **X_min** to shift the minimum to 0.  
- Divide by the range (X_max − X_min) to scale the maximum to 1.  
- Result: All values lie between 0 and 1.

---

## 2. Z-score Standardization (Standard Scaling)

**Formula:**
X_norm = (X - μ) / σ

| Symbol           | Meaning                                              |
|-----------------|------------------------------------------------------|
| X               | Original value of the feature                          |
| μ (mu)          | Mean of the feature values in the dataset           |
| σ (sigma)       | Standard deviation of the feature values            |
| X_norm          | Normalized value with mean 0 and standard deviation 1|

**Explanation:**  
- Subtract **mean (μ)** to center data around 0.  
- Divide by **standard deviation (σ)** to scale spread to 1.  

---

## 3. Max-Abs Scaling

**Formula:**
X_norm = X / |X_max|


| Symbol           | Meaning                                              |
|-----------------|------------------------------------------------------|
| X               | Original value of the feature                          |
| X_max           | Maximum absolute value of the feature               |
| X_norm          | Normalized value scaled to [-1, 1]                  |

---

## 4. Robust Scaling

**Formula:**
X_norm = (X - median) / IQR


| Symbol           | Meaning                                              |
|-----------------|------------------------------------------------------|
| X               | Original value of the feature                          |
| median          | Median value of the feature                          |
| IQR             | Interquartile range (Q3 − Q1)                        |
| X_norm          | Normalized value resistant to outliers               |

---

**Summary of Symbols:**

| Symbol           | Meaning                                              |
|-----------------|------------------------------------------------------|
| X               | Original value of the feature                          |
| X_min           | Minimum value of the feature                           |
| X_max           | Maximum value of the feature                           |
| μ               | Mean of the feature                                    |
| σ               | Standard deviation of the feature                      |
| median          | Median of the feature                                   |
| IQR             | Interquartile range (Q3 − Q1)                          |
| X_norm          | Normalized value                                       |

----

