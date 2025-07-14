# 🧹 EDA and Preprocessing

## 📌 Objective

The main objective of this project is to design and implement a robust **data preprocessing system** that addresses common challenges such as:

- Missing values
- Outliers
- Inconsistent formatting
- Noise

## 📂 Dataset

- Source: [Click here to access the dataset](https://drive.google.com/file/d/1F3lRf32JM8ejnXq-Cbf9y7fa57zSHGz_/view?usp=sharing)
- Format: CSV
- Contains information like employee name, age, salary, city, gender, etc.

## ✅ Key Components & Steps

### 1. 📊 Data Exploration 
- Displayed basic structure and info using `df.info()` and `df.describe()`
- Counted and listed unique values in each column using `df.nunique()` 
- Renamed columns for better readability and to remove inconsistencies

### 2. 🧼 Data Cleaning 
- Replaced inappropriate values like `0` in `employee_age` with `NaN`
- Handled missing values using:
  - **Median** for numerical columns (e.g., `employee_age`, `monthly_salary`)
  - **Unknown** for categorical columns (e.g., `company_name`, `city`)
- Removed all duplicate rows
- Detected and visualized outliers using box plots

### 3. 📈 Data Analysis 
- Filtered data: `employee_age > 40` and `monthly_salary < 5000`
- Visualized relationship between Age and Salary using scatter plots
- Counted people from each city and represented it using bar plots

### 4. 🧠 Data Encoding 
- Used **One-Hot Encoding** for multi-class categorical variables like `city`

### 5. 📐 Feature Scaling 
- Applied both:
  - **StandardScaler** (Z-score normalization)
  - **MinMaxScaler** (0–1 scaling)
- Stored results in separate DataFrames to preserve original data
- 

## 📊 Visualizations Included

- Box plots to identify outliers
- Scatter plot of Age vs Salary
- Bar chart of population count by place

## 🧾 Tools & Libraries Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-learn


## 📁 Files in This Repository

| File/Folder | Description |
|-------------|-------------|
| `EDA_and_Preprocessing.ipynb` | Main Jupyter Notebook |
| `README.md` | This file |
| `Employee.csv` | Input dataset  |

