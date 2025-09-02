# What is EDA?

**EDA** stands for **Exploratory Data Analysis**.  
It’s the process of **exploring and understanding the dataset** before applying any machine learning or statistical models.  

The goal is simple: **get to know the data.**  
Just like a doctor does a basic check-up before treatment, EDA is a check-up for the dataset.

---

## Why do EDA?
- To **understand what’s in the data** (size, shape, types of values).  
- To **spot problems** like missing values, duplicates, or strange outliers.  
- To **see patterns** that could be useful for prediction.  
- To **decide next steps**: cleaning, feature engineering, or even redefining the problem.  

---

## Types of EDA
EDA can be done in different ways depending on what we want to discover:

1. **Univariate Analysis**  
   - Focuses on a **single column** at a time.  
   - Example: Plotting the distribution of "age" with a histogram.  
   - Goal: Understand spread, central tendency, and outliers.  

2. **Bivariate Analysis**  
   - Looks at the **relationship between two variables**.  
   - Example: Scatterplot of "house price" vs. "size in square feet".  
   - Goal: Find correlations or patterns between pairs of columns.  

3. **Multivariate Analysis**  
   - Studies **more than two variables together**.  
   - Example: How "income", "education level", and "age" together affect "spending habits".  
   - Goal: Detect interactions and complex relationships.  

4. **Graphical (Visual) EDA**  
   - Uses charts: histograms, boxplots, scatterplots, heatmaps.  
   - Goal: Quickly spot patterns, clusters, and anomalies.  

5. **Non-Graphical (Statistical) EDA**  
   - Uses numbers: mean, median, standard deviation, correlation coefficients.  
   - Goal: Summarize data mathematically without visual plots.  

---

## Typical Steps in EDA
1. **Basic info** → How big is the dataset (rows & columns)? What are the column names?  
2. **Preview data** → Look at a few random rows with `.sample()` to get a quick feel.  
3. **Data types** → Identify numeric, categorical, text, or datetime columns.  
4. **Missing values** → Check how many values are missing and where.  
5. **Summary stats** → Mean, median, min, max, standard deviation.  
6. **Duplicates** → See if rows repeat unnecessarily.  
7. **Correlations** → Spot relationships between numeric columns.  
8. **Visualizations** → Use histograms, scatterplots, and boxplots to see distributions and patterns.  

---

## Quick Analogy
- Think of EDA as **meeting a new person**.  
- You first ask basic questions (name, age, background).  
- Then you notice patterns (hobbies, interests).  
- You might also spot red flags (inconsistencies, missing info).  
- Only after knowing them well do you make decisions (like whether you want to work together).  

---

📌 *EDA is not about building models. It’s about building understanding.*
