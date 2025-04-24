# 🚢 Titanic Dataset – Data Preprocessing Project

This project was completed in **Google Colab** as part of an **AI & ML internship**. It focuses on preparing the Titanic dataset for machine learning by handling missing data, encoding categorical features, normalizing numerical columns, and identifying/removing outliers.

---

## 📂 Dataset Used
- [Titanic Dataset (Kaggle)](https://www.kaggle.com/c/titanic/data)
- File name: `Titanic-Dataset.csv`

---

## ✅ Steps Performed

### 1. 📥 Importing Libraries & Loading Dataset
- Imported `pandas`, `numpy`, `seaborn`, `matplotlib`, and `sklearn`.
- Loaded the dataset using `pd.read_csv()` and explored with:
  ```python

  2. 🧼 Handling Missing Values
Filled missing values using appropriate imputation:
Age: filled with median
Fare: filled with mean
Embarked: filled with mode
Cabin: replaced with "Unknown"

3. 🔢 Encoding Categorical Features
Label Encoded the Sex column: male → 0, female → 1
Applied One-Hot Encoding to Embarked
pd.get_dummies(df, columns=['Embarked'], drop_first=True)

4. 📐 Normalization & Standardization
Detected all numeric columns automatically using select_dtypes()
Standardized all numeric features using StandardScaler
Also normalized using MinMaxScaler (for comparison)

5. 📊 Outlier Visualization with Boxplots
Plotted boxplots for the following columns to visually inspect outliers:
Age
SibSp
Fare
Parch


🛠️ Tools & Libraries
Google Colab (Python 3)
Pandas, Numpy
Matplotlib, Seaborn
Scikit-learn

📁 Project Files
Titanic-Dataset.csv → Original dataset

titanic_preprocessing.ipynb → Google Colab notebook

README.md → Project documentation (this file)


