# 🎓 Nobel Prize Data Analysis — Python Project  
A clean, insightful and beginner-friendly **Data Analysis project** built using **Pandas, NumPy, and Seaborn**.  
This project explores the Nobel Prize dataset to uncover trends such as gender distribution, country dominance, female laureates, and historical patterns across decades.

---

## 📌 Project Overview

In this project, we analyze the **Nobel Prize dataset** to answer important questions:

1. **Most commonly awarded gender**  
2. **Most common birth country of Nobel laureates**  
3. **Decade with highest ratio of US-born Nobel winners**  
4. **Decade & category with highest female laureate proportion**  
5. **First woman to win a Nobel Prize**  
6. **Individuals who received multiple Nobel Prizes**

This project helps you understand:
- Data cleaning  
- GroupBy operations  
- Ratios & proportions  
- Handling missing values  
- Exploratory Data Analysis (EDA)

---

## 🧰 Tech Stack
- **Python**
- **Pandas**
- **NumPy**
- **Seaborn**  
- **Jupyter Notebook / VS Code**

---

## 📂 Dataset
The project uses **nobel.csv**, which contains detailed historical Nobel Prize winner records with the following columns:

- **year**
- **category**
- **prize**
- **motivation**
- **prize_share**
- **laureate_id**
- **laureate_type**
- **full_name**
- **birth_date**
- **birth_city**
- **birth_country**
- **sex**
- **organization_name**
- **organization_city**
- **organization_country**
- **death_date**
- **death_city**
- **death_country**

This dataset provides rich information for performing gender analysis, country trends, organization patterns, and lifetime details of Nobel laureates.


## 🚀 Key Insights

### ✔️ 1. Most Common Gender & Birth Country  
The analysis identifies the **most awarded gender** and **most frequent birth country**.

### ✔️ 2. US Dominance by Decade  
Calculates the **ratio of US-born winners per decade** and finds the decade with the highest influence.

### ✔️ 3. Female Laureate Trends  
Finds the **decade and category** with the highest proportion of female winners.

### ✔️ 4. First Woman Nobel Winner  
Extracts the name & category of the **first female Nobel Prize winner**.

### ✔️ 5. Multiple-Time Laureates  
Lists the individuals/organizations that won the Nobel Prize **more than once**.

---

## 🧪 Code Structure (High Level)

```python
df = pd.read_csv("data/nobel.csv")          # Load dataset
df.info()                                   # Dataset summary
df.isnull().sum()                           # Missing values check

df['decade'] = (df['year'] // 10) * 10      # Create decade column