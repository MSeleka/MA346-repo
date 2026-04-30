# 🏀 NBA Player Performance and Salary Analysis (2025–26)

## 📊 Project Overview
This project analyzes the relationship between NBA player performance and salary during the 2025–26 season. The goal is to determine whether higher-performing players tend to earn higher salaries, and to identify which performance metrics are most strongly associated with compensation.

The analysis combines player performance data with salary data to create a unified dataset, enabling statistical modeling and data-driven insights into salary determination.

---

## 🎯 Key Questions
- How strongly is player performance related to salary?
- Which performance metrics (points, assists, rebounds, minutes played) best explain salary?
- How much of salary variation can be explained by observable performance?

---

## 🗂️ Data Sources
- **Performance Data:** Stathead Basketball (Sports Reference)
- **Salary Data:** Basketball-Reference

These datasets were merged on player name and season to create a single dataset containing both performance metrics and salary information for each player.

---

## 🧹 Data Preparation
- Cleaned column names and standardized formatting
- Removed unnecessary variables
- Fixed inconsistencies in player names
- Converted salary from string format to numeric
- Removed duplicates and handled missing values
- Merged datasets using an inner join on player and season

---

## 📈 Methods Used
The project applies both statistical and data science techniques:

### 🔹 Exploratory Data Analysis (EDA)
- Distribution of salaries
- Scatterplots (salary vs performance metrics)
- Correlation analysis
- Boxplots by scoring tiers

### 🔹 Statistical Modeling
- **Linear Regression (OLS)**  
  - Simple model: Salary ~ Points  
  - Multiple model: Salary ~ PTS + AST + TRB + MP  
- **ANOVA** (feature significance)
- **Quantile Regression** (distribution-sensitive modeling)
- **Residual Analysis** (model diagnostics)

---

## 📊 Key Findings
- Player performance is strongly associated with salary
- **Points (scoring)** is the most important predictor
- Performance metrics explain about **58% of salary variation**
- Additional variables (assists, rebounds) improve the model modestly
- Residual analysis shows **heteroskedasticity**, meaning prediction error increases for higher salaries
- Salary is influenced by factors beyond performance, such as:
  - Experience and contract structure
  - Team role and usage
  - Reputation and market dynamics

---

## 🧠 Interpretation
While performance metrics provide meaningful insight into salary, they do not fully explain compensation. The results suggest that NBA salaries reflect both measurable performance and external factors not captured in the dataset.

