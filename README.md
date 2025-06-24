# AI-ML-Task-2

### By Abhishek Mitra

# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

## 📌 Objective
To understand the structure, patterns, and insights in the Titanic dataset using descriptive statistics and visualizations.

---

## 📂 Dataset Overview
- **Rows:** 851 passengers
- **Features:** `PassengerId`, `Survived`, `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked_Q`, `Embarked_S`
- **Note:** Some features are one-hot encoded and some are normalized (like `Age` and `Fare`).

---

## 🔍 Tasks Completed

### ✅ 1. Summary Statistics

Used `pandas.describe()` to get:
- Central tendencies (mean, median)
- Spread (standard deviation)
- Min, max, and quartiles

### ✅ 2. Visualizations

#### 📊 Histograms
Plotted for all numeric features to visualize distributions and skewness.

#### 📦 Boxplots
Used to detect outliers and spread:
- `Fare` and `Age` showed noticeable outliers.
- `SibSp` and `Parch` had right-skewed distributions.

#### 🔗 Correlation Matrix
Generated using `.corr()` and plotted as a heatmap using Seaborn.
- Showed positive correlation between `Fare` and `Survived`.
- Negative correlation between `Sex` (1 = male) and `Survived`.

#### 🔄 Pairplot
Visualized interactions between `Survived`, `Pclass`, `Sex`, `Age`, and `Fare`.

---

## 📈 Patterns, Trends, and Anomalies

### ✔ Patterns:
- **Survival by Gender**:  
  ✅ *Females had a higher survival rate than males.*

- **Survival by Class**:  
  ✅ *Passengers in class 1 had the highest survival rate.*

- **Fare vs Survival**:  
  ✅ *Higher fare is positively correlated with survival.*

### ⚠ Anomalies:
- **Age**:  
  ⛔ Some extreme outliers present after normalization (e.g., values below -2 or above +2).

- **Embarkment**:  
  ✅ *Most passengers embarked from port `S`.*

---

## 🧠 Inference Summary

| Feature      | Inference |
|--------------|-----------|
| Sex          | Females had significantly higher survival chances |
| Pclass       | 1st Class passengers survived more often |
| Fare         | Higher-paying passengers were more likely to survive |
| Age          | Some unusual/extreme values suggest data anomalies |
| Embarked_S   | Most passengers boarded at port S |

---

## 📎 Tools Used

- **Pandas** – for data manipulation and statistics
- **Matplotlib** & **Seaborn** – for plotting histograms, boxplots, heatmaps, and pairplots
- **Jupyter Notebook** – for interactive analysis

---

## ✅ Status
✔ Completed core EDA task as part of the internship assignment.  
📁 Notebook Name: `Titanic_EDA_Internship_Abhishek.ipynb`

---

> Prepared by: **Abhishek M.**  
> Internship Task – June 2025  

