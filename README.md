# 🏨 Hotel Booking Data Cleaning Project

## 📌 Objective
The goal of this project is to build a **robust data preprocessing pipeline** for a hotel booking cancellation prediction model.  
The quality of data cleaning directly determines the future success of the machine learning model.

---

## 📂 Files in Repository
- `hotel_bookings.csv` → Raw dataset used for analysis  
- `notebook.ipynb` → Jupyter Notebook containing all preprocessing steps  
- `README.md` → Project documentation  

---

## 🔧 Data Cleaning Steps Performed
1. **Exploratory Data Analysis (EDA)**
   - Used `.info()` and `.describe()` to understand dataset  
   - Checked for missing values and data types  

2. **Missing Values Handling**
   - `agent` and `company`: Replaced NaN with `0`  
   - `country`: Filled missing values with the **mode (most frequent country)**  

3. **Duplicate Records**
   - Removed exact duplicate rows  

4. **Outlier Treatment**
   - Capped `adr` (Average Daily Rate) at **1000** to avoid extreme skew  
   - Used boxplots and IQR method for detection  

5. **Data Type Fixing**
   - Converted `reservation_status_date` to `datetime`  

6. **High Cardinality Features**
   - Grouped infrequent `country` categories into **"Other"**  

7. **Categorical Inconsistencies**
   - Standardized inconsistent categorical entries  

---

## 📊 Key Findings
- Dataset had **missing values** in `agent`, `company`, and `country`  
- `adr` column contained **extreme outliers**  
- Duplicate rows existed and were removed  
- After cleaning, data is now **ready for machine learning models**  

---

## 🚀 How to Use
1. Open the notebook in **Google Colab** or **Jupyter Notebook**  
2. Run all cells to reproduce preprocessing pipeline  
3. Use the cleaned dataset for future ML modeling  

---

## ✨ Author
Prepared by: **[Your Name]**  
For: **Hotel Booking Cancellation Prediction - Data Preprocessing**
