#  EXPERIMENT – 14  
# DATA NORMALIZATION AND DATA TYPE CONVERSION USING PYTHON  

---

##  STUDENT DETAILS  

**Name:** Asit Kumar Srivastava  
**PRN:** 25070123026  
**Batch:** A2 (ENTC)  
**Subject:** Exploratory Data Analysis using Python  

---

##  AIM  

To perform **Data Normalization and Data Type Conversion** using Python and understand their importance in data preprocessing for analysis and machine learning.

---

## 🎓 OBJECTIVES  

• To understand the concept of data normalization  
• To implement Min-Max, Z-score, and Decimal Scaling normalization  
• To perform encoding techniques for categorical data  
• To convert raw data into machine-readable format  
• To prepare datasets for analysis and predictive modeling  

---

## 📚 THEORY  

### 🔹 Data Normalization  

Data Normalization is the process of **scaling numerical values** into a specific range without distorting differences in the data.

It helps in:
• Improving model performance  
• Reducing bias due to large values  
• Ensuring uniform data distribution  

---

### 🔹 Types of Normalization  

#### 1️⃣ Min-Max Normalization  

Scales values between 0 and 1.

Formula:

```python
(x - min) / (max - min)
```

---

#### 2️⃣ Z-Score Normalization  

Transforms data based on mean and standard deviation.

Formula:

```python
(x - mean) / standard deviation
```

---

#### 3️⃣ Decimal Scaling  

Moves decimal point to scale values.

Formula:

```python
x / 10^n
```

---

### 🔹 Data Type Conversion  

Data Type Conversion is the process of converting categorical data into numerical form.

It is required because:
• Machine learning models only understand numbers  
• Improves data consistency  
• Enables mathematical operations  

---

### 🔹 Encoding Techniques  

#### 1️⃣ Label Encoding  

Converts categories into numeric labels.

Example:
Male → 0  
Female → 1  

---

#### 2️⃣ One-Hot Encoding  

Creates separate binary columns for each category.

---

#### 3️⃣ Dummy Encoding  

Similar to One-Hot Encoding but drops one column to avoid redundancy.

---

## 🧠 METHODOLOGY / IMPLEMENTATION  

### 🔸 PART A: DATA NORMALIZATION  

#### Step 1: Dataset Creation  

Dataset includes:
- Product  
- Price  
- Units Sold  
- Discount  

---

#### Step 2: Min-Max Normalization  

Applied on:
• Price  
• Units Sold  
• Discount  

```python
(df[col] - df[col].min()) / (df[col].max() - df[col].min())
```

---

#### Step 3: Z-Score Normalization  

Applied on Units Sold:

```python
(df[col] - df[col].mean()) / df[col].std()
```

---

#### Step 4: Decimal Scaling  

```python
df[col] / scaling_factor
```

---

#### Step 5: Normalizing Multiple Columns  

Multiple attributes normalized simultaneously for consistency.

---

### 🔸 PART B: DATA TYPE CONVERSION  

#### Step 1: Dataset Creation  

Dataset includes:
- Order ID  
- Gender  
- Payment Method  
- Product Category  
- City  
- Order Value  

---

#### Step 2: Label Encoding  

```python
from sklearn.preprocessing import LabelEncoder
```

Applied on Gender.

---

#### Step 3: One-Hot Encoding  

```python
pd.get_dummies()
```

Applied on:
• Product Method  
• Product Category  
• City  

---

#### Step 4: Dummy Encoding  

```python
pd.get_dummies(drop_first=True)
```

Reduces multicollinearity.

---

### 🔸 PART C: REAL DATASET OPERATIONS  

• Dataset loaded using CSV file  
• Multiple normalization techniques applied  
• Encoding performed on student dataset  

---

## ⚙️ KEY LIBRARIES USED  

```python
pandas
numpy
sklearn.preprocessing
```

---

## 📊 OBSERVATIONS  

• Min-Max normalization scales values between 0 and 1  
• Z-score normalization centers data around mean  
• Decimal scaling reduces magnitude of values  
• Encoding converts categorical data into numerical form  
• One-Hot Encoding increases dimensionality  
• Dummy Encoding prevents redundancy  

---

## ✅ RESULT  

Data Normalization and Data Type Conversion techniques were successfully implemented.  
The dataset was transformed into a structured, consistent, and machine-readable format.

---

## 💡 LEARNING OUTCOMES  

• Understood importance of data preprocessing  
• Learned multiple normalization techniques  
• Implemented encoding for categorical data  
• Gained practical knowledge of preparing datasets for ML models  

---

## 📎 SOURCE CODE  

Complete implementation is available in this repository.  

(Source: :contentReference[oaicite:0]{index=0})

---
## 🔍 PROJECT SIGNIFICANCE  

This experiment demonstrates:  
• Practical implementation of data preprocessing techniques  
• Application of normalization methods for numerical data  
• Effective handling of categorical data through encoding  
• Preparation of datasets for machine learning and analytical tasks  



