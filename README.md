
# **Exploratory Data Analysis – Dealing with Null Values in Python**


This project demonstrates how to identify and handle missing values in a real-world dataset (`snsdata.csv`) using Python's pandas library.

---

## 📁 Dataset Used

- **snsdata.csv**: A social networking dataset containing demographic and interest-related information such as:
  - `gender`
  - `age`
  - `gradyear`
  - `friends`
  - and other user interests.

---

## 🔍 What This Project Covers

| Step | Description |
|------|-------------|
| 1️⃣ | Reading the dataset using `pandas.read_csv()` |
| 2️⃣ | Checking for missing values using `isna()`, `isnull()` |
| 3️⃣ | Counting missing vs non-missing values using `.sum()` |
| 4️⃣ | Exploring complete data with `.info()` |
| 5️⃣ | Comparing `isna()` vs `isnull()` and `notna()` vs `notnull()` |
| 6️⃣ | Understanding the structure and memory usage of the dataset |

---

## 📌 Key Pandas Functions Explained

| Function | Purpose |
|----------|---------|
| `isna()` | Detect missing (null) values |
| `isnull()` | Same as `isna()` |
| `notna()` | Detect non-missing (non-null) values |
| `notnull()` | Same as `notna()` |
| `.sum()` | Count how many `True` values (i.e. missing or non-missing) |
| `.info()` | Overview of DataFrame (column types, non-null counts, memory usage) |

---

## 🧠 Insights You Can Gain

- Which columns have missing data?
- How many missing values exist in each column?
- What's the total memory footprint of your dataset?
- What's the data type of each column?
- How to confidently clean and prepare data before model building.

---

## 🛠 Tools Used

- **Python 3.x**
- **Pandas**
- **Jupyter Notebook**

---

## 📷 Sample Output

```python
snsdata.gender.isna().sum()   # e.g. 30 missing gender values
snsdata.age.isna().sum()      # e.g. 45 missing age values
cars.isnull().sum()           # Check missing in another dataset
cars.notnull().sum()          # Count non-missing values
