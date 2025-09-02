# Basic Questions for Understanding the Data

When I first look at a dataset, I ask myself some simple but important questions:

---

### 1. How big is the data?  
- How many **rows** (examples) are there?  
- How many **columns** (features/variables) are there?  
- Is the dataset small enough to load in memory, or do I need special tools for big data?

---

### 2. How does the data look like?  
- Instead of always using `.head()` (which shows the first few rows), I prefer `.sample()` to see **random rows** from the dataset.  
- This gives me a less biased view of how the data looks.  
- Do the values seem reasonable (e.g., no negative ages, no empty strings)?  

---

### 3. What are the data types of the columns?  
- Are columns **numeric** (integers, floats), **categorical** (labels like “male/female”), **datetime**, **text**, or **boolean**?  
- This matters because different algorithms handle data types differently.  

---

### 4. Are there any missing values?  
- Which columns have missing entries?  
- How many are missing (a few or a lot)?  
- Should I drop them, fill them (impute), or keep them as-is?  

💡 *Imputation = replacing missing values with estimates, like mean, median, or a special category.*

---

### 5. How does the data look mathematically?  
- Summary statistics: mean, median, min, max, standard deviation.  
- Do values fall into expected ranges?  
- Are there extreme **outliers** (unusually high/low values)?  

---

### 6. Are there duplicate values?  
- Do any rows repeat?  
- If yes, should I drop them or keep them (depends on the context)?  

---

### 7. Correlation between columns  
- Which columns are strongly related to each other?  
- Are some features redundant (too similar)?  
- Which features seem most related to the target (the thing I want to predict)?  

---

## ✅ Quick Checklist
- [ ] Size: number of rows and columns  
- [ ] First look at the data (with `.sample()` for random rows)  
- [ ] Data types of each column  
- [ ] Missing values  
- [ ] Summary statistics (mean, median, outliers)  
- [ ] Duplicate rows  
- [ ] Correlations between features  

---

📌 *Asking these questions helps me “get to know” the dataset before I even think about building a model. It’s like doing a health check on the data.*
