# EDA Using Univariate Analysis

**Univariate Analysis** is about exploring **one column (feature) at a time** in the dataset.  
The goal is to **understand its distribution, central values, spread, and any unusual values (outliers)**.

---

## 1. Why Univariate Analysis?
- To see the **distribution** of values (how data is spread).  
- To find **central tendency** (typical value) like mean, median, and mode.  
- To detect **outliers** (values that are unusually high or low).  
- To check **data quality** (missing values, wrong data types).

---

## 2. Numeric Columns
For numeric features (numbers), we usually check:

1. **Summary statistics**  
   - Mean, median, minimum, maximum, standard deviation, quartiles.  
   - Helps understand the **range** and **variation** of values.

2. **Visualizations**  
   - **Histogram** → Shows how values are distributed.  
   - **Boxplot** → Highlights median, quartiles, and outliers.  

*Example Questions:*  
- What is the average age of customers?  
- Are there any extremely high or low salaries in the dataset?  

---

## 3. Categorical Columns
For categorical features (labels), we usually check:

1. **Frequency count**  
   - How many times each category appears (value counts).  

2. **Visualizations**  
   - **Bar plot** → Shows the count of each category.  

*Example Questions:*  
- How many customers are male vs female?  
- Which product category has the highest sales?  

---

## 4. Steps for Univariate Analysis
1. Pick a column (numeric or categorical).  
2. Check **summary statistics** (`describe()` for numeric, `value_counts()` for categorical).  
3. Visualize the column (histogram for numeric, bar plot for categorical).  
4. Look for **missing values, outliers, or strange patterns**.  
5. Repeat for each column in the dataset.  

---

## 5. Quick Analogy
- Think of univariate analysis as **examining one ingredient in a recipe** before cooking.  
- You check its color, smell, quantity, and quality individually before mixing it with others.  

---

📌 *Univariate analysis is the first step in EDA. It gives a solid understanding of each feature on its own, which helps later for bivariate and multivariate analysis.*
