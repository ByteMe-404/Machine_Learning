# Feature Encding 

Feature encoding converts categorical data into numerical representations so machine learning algorithms can process them.

---

## 1. Label Encoding
**When to use :**
-Categorical features has **ordinal relationship** (e.g. , low < medium < high ).
-Algorithms like **tree-based models** or linear models that can handle integers.

**Notes:**
- Converts categories to integers (0, 1, 2, …).  
- Beware: introduces artificial ordinal relationship if data is nominal.
- Only use in output columns.
---

## 2. One-Hot Encoding

**When to Use:**
- Categorical feature is **nominal** (no order) and has **few unique categories**.  
- Algorithms sensitive to numeric magnitude (e.g., Linear Regression, KNN, Neural Networks).

**Notes:**
- Creates new binary columns for each category.  
- Can cause **dimensionality explosion** if too many categories.

---

## 3. Ordinal Encoding

**When to Use:**
- Categories have a natural order (e.g., rating: Poor < Average < Good < Excellent).  
- Similar to label encoding but preserves **specified order**.

**Notes:**
- Map categories explicitly to numbers (e.g., Poor=1, Average=2, Good=3, Excellent=4).  

---

## 4. Target Encoding (Mean Encoding)

**When to Use:**
- High-cardinality categorical features (many unique values).  
- Regression or classification tasks.

**Notes:**
- Replace category with **mean of target variable** for that category.  
- Be careful of **data leakage**: compute mapping on training data and apply to test set.

---

## 5. Frequency / Count Encoding

**When to Use:**
- High-cardinality categorical features.  
- Simple method that captures **category popularity**.

**Notes:**
- Replace category with count or frequency in the dataset.  
- Works well with tree-based models.

---

## Quick Decision Table

| Encoding Type       | Best For                                        | Notes                                      |
|-------------------|-------------------------------------------------|-------------------------------------------|
| Label Encoding      | Ordinal categories                              | Beware of artificial order for nominal    |
| One-Hot Encoding    | Nominal categories with few unique values       | Can increase dimensionality               |
| Ordinal Encoding    | Categories with natural order                   | Specify order explicitly                  |
| Target/Mean Encoding| High-cardinality features                        | Avoid data leakage                         |
| Frequency Encoding  | High-cardinality features                        | Captures category popularity              |
