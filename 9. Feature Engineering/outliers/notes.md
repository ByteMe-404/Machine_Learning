# 📊 Outliers in Data

## 🔹 What are Outliers?
An **outlier** is a data point that is significantly different from the rest of the dataset.  
They may be errors, rare events, or unusual but valid observations.  

---

## 🔹 Why Do Outliers Matter?
- Skew statistical measures (mean, variance, regression).  
- Indicate anomalies (fraud, equipment failure).  
- Help check data quality.  

---

## 🔹 Types of Outliers
1. **Univariate Outlier** – unusual in one variable.  
2. **Multivariate Outlier** – unusual combination across multiple variables.  
3. **Global Outlier** – far from the whole dataset.  
4. **Contextual Outlier** – unusual in a specific context (e.g., 30°C in winter).  
5. **Collective Outlier** – a group of unusual values together.  

---

## 🔹 Causes of Outliers
- Data entry or measurement errors  
- Sampling errors  
- Natural variability  
- Experimental setup issues  

---

## 🔹 How to Detect Outliers
### 1. Statistical Methods
- **Z-score method**: values more than 3 standard deviations from the mean.  
- **IQR (Interquartile Range) method**: values outside Q1 – 1.5×IQR or Q3 + 1.5×IQR.  

### 2. Visualization Methods
- **Boxplot** → outliers appear as isolated points.  
- **Histogram** → extreme values show as far bars.  
- **Scatter plot** → detects unusual points in 2D/3D.  

### 3. Machine Learning Methods
- **Isolation Forest**  
- **DBSCAN (clustering)**  
- **One-class SVM**  

---

## 🔹 How to Handle Outliers
1. **Investigate** → If error, correct or remove.  
2. **Transform data** → Log, square root, or Box-Cox.  
3. **Use robust statistics** → Median, IQR instead of mean, variance.  
4. **Cap or Winsorize** → Limit extreme values.  
5. **Keep them** → If they represent meaningful anomalies (fraud, rare events).  

---

## 🔹 Example
Dataset: `[45, 50, 48, 52, 47, 95]`  
- Mean = 56  
- The value **95** is far from the rest → an outlier.  

---

✅ **Summary:** Outliers are extreme values that can distort analysis, but they can also reveal important insights.
