# Feature Scaling Cheat Sheet (When to Use)

Feature scaling ensures that numerical features contribute equally to machine learning models.

---

## 1. Min-Max Scaling

**When to Use:**
- All features need to be in a fixed range [0,1].
- Algorithms sensitive to magnitude, e.g., Neural Networks, KNN, SVM (RBF kernel).
- Data does **not** have extreme outliers.

---

## 2. Standard Scaling (Z-score Normalization)

**When to Use:**
- Data may have outliers.
- Algorithms that assume features centered around 0: Linear Regression, Logistic Regression, PCA, SVM.
- You want unit variance across features.

---

## 3. Robust Scaling

**When to Use:**
- Data contains extreme outliers.
- You want a scale less sensitive to outliers.
- Useful for skewed distributions.

---

## 4. Max-Abs Scaling

**When to Use:**
- Data is already centered at 0 or mostly positive.
- Sparse data in linear models.
- Preserving sparsity is important.

---

## Quick Decision Table

| Scaler             | Best For                                         | Notes                                     |
|-------------------|--------------------------------------------------|------------------------------------------|
| Min-Max            | Neural Networks, KNN, SVM                       | Sensitive to outliers                     |
| StandardScaler     | Linear models, PCA, gradient descent, SVM      | Assumes Gaussian-like distribution        |
| RobustScaler       | Data with outliers                              | Centers around median, uses IQR           |
| MaxAbsScaler       | Sparse data, already centered around 0          | Preserves sparsity, sensitive to outliers |
