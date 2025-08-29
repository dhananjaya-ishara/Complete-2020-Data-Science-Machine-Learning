# Complete-2020-Data-Science-Machine-Learning(reading)

1st -Linear_Regrassion.ipynb and dataset cost_revenue_clean.csv
2nd -  Variables and Types ,lsd_math_score_data.csv, Lists and Arrays ,Dataframes and Series,Module Imports(3_Python_Programming_for_Data_Science_and_Machine_Learningintro.ipynb)
3rd-python function ,Funcction.ipynb
4th-Objects&Attribute&code_style_and_naming_conventions.ipynb,life.py
5th-LaTeX Markdown and Generating Data with Numpy(that in clude cost funtion,slope of the cost function,gradient descent(closeup))


Got it 👍 You can clean and drop rows in an **Excel file using Python (pandas)**. Here are the main steps and examples:

---

### ✅ 1. Load Excel file

```python
import pandas as pd

# Read Excel file
df = pd.read_excel("your_file.xlsx")
```

---

### ✅ 2. Drop rows with **missing values (NaN)**

```python
# Drop rows where ANY column has a missing value
df = df.dropna()

# Drop rows where ALL values are missing
df = df.dropna(how='all')

# Drop rows where specific column(s) have missing values
df = df.dropna(subset=['ColumnName'])
```

---

### ✅ 3. Drop rows with **duplicate values**

```python
# Drop duplicate rows
df = df.drop_duplicates()

# Drop duplicates based on specific column(s)
df = df.drop_duplicates(subset=['ColumnName'])
```

---

### ✅ 4. Drop rows based on a **condition**

```python
# Drop rows where column value equals something
df = df[df['ColumnName'] != 'UnwantedValue']

# Drop rows where column value is greater/less than a threshold
df = df[df['Age'] > 18]   # keep only rows where Age > 18
```

---

### ✅ 5. Save cleaned data back to Excel

```python
# Save the cleaned dataframe into a new Excel file
df.to_excel("cleaned_file.xlsx", index=False)
```

---

👉 So in short:

* `dropna()` → remove missing values
* `drop_duplicates()` → remove duplicate rows
* Boolean filtering (`df[df['Column'] != value]`) → remove rows by condition

Do you want me to prepare a **ready-made cleaning script** where you can just replace the Excel file name and column names, and it will automatically drop NaN, duplicates, and inconsistent values?
