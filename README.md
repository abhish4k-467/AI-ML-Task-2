# AI-ML-Task-2 -> Exploratory Data Analysis

### By Abhishek Mitra

#### 📎 Tools Used

- **Pandas** – for data manipulation and statistics
- **Matplotlib** & **Seaborn** – for plotting histograms, boxplots, heatmaps, and pairplots
- **Jupyter Notebook** – for interactive analysis

# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

## 📌 Objective
To understand the structure, patterns, and insights in the Titanic dataset using descriptive statistics and visualizations.

---

## 📂 Dataset Overview
- **Rows:** 891 passengers
- **Features:**  `Survived`, `Pclass`, `Sex`, `Age`, `SibSp`, `Parch`, `Fare`, `Embarked_Q`, `Embarked_S`
---

## 🔍 Tasks Completed

### ✅ 1. Summary Statistics

Used `df.describe()` to get:
- Central tendencies (mean, median)
- Spread (standard deviation)
- Min, max, and quartiles

  ![image](https://github.com/user-attachments/assets/0a02e434-01ea-41e7-b096-0743170b58c2)



### ✅ 2. Visualizations

#### 📊 Histograms
Plotted for all numeric features to visualize distributions and skewness.

![image](https://github.com/user-attachments/assets/bd67de62-284e-4694-8f3d-4a8f1335660b)


#### 📦 Boxplots
Used to detect outliers and spread:
- `Fare` and `Age` showed noticeable outliers.

  ![image](https://github.com/user-attachments/assets/2e8d4f93-a260-4eb4-8a25-e83e28d1cafe)

  ![image](https://github.com/user-attachments/assets/4220aa1c-82a3-4e51-ad29-d80574fe84f2)

#### 🔗 Correlation Matrix
Generated using `.corr()` and plotted as a heatmap using Seaborn.
- Showed positive correlation between `Fare` and `Survived`.
- Negative correlation between `Sex` (1 = male) and `Survived`.

  ![image](https://github.com/user-attachments/assets/e8fd004c-932f-463d-8203-84f49e4d8b58)


#### 🔄 Pairplot
Visualized interactions between `Survived`, `Pclass`, `Sex`, `Age`, and `Fare`.


![image](https://github.com/user-attachments/assets/46776486-98ef-4f12-b398-e638d604675a)


---

## 📈 Patterns, Trends, and Anomalies

### ✔ Patterns:
- **Survival by Gender**:  
  ✅ *Females had a higher survival rate than males.*

- **Survival by Class**:  
  ✅ *Passengers in class 1 had the highest survival rate.*

- **Fare vs Survival**:  
  ✅ *Higher fare is positively correlated with survival.*

- **Embarkment**:  
  ✅ *Most passengers embarked from port `S`.*

---

## 🧠 Inference Summary

| Feature      | Inference |
|--------------|-----------|
| Sex          | Females had significantly higher survival chances |
| Pclass       | 1st Class passengers survived more often |
| Fare         | Higher-paying passengers were more likely to survive |
| Embarked_S   | Most passengers boarded at port S |
