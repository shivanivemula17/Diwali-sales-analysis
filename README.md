# Diwali-sales-analysis
This repository contains a Diwali Sales Analysis project, focusing on data cleaning, exploratory data analysis (EDA), and visualization. Using Python libraries like Pandas, Matplotlib, and Seaborn
# 🎇 Diwali Sales Analysis  

## 📌 Project Overview  
This project analyzes **Diwali sales data** to uncover **consumer behavior, top-selling products, revenue trends, and demographics**. The goal is to identify purchasing patterns and optimize future sales strategies.  

## 🔍 Key Features  
✔️ **Cleaned & pre-processed the dataset** to remove inconsistencies and missing values.  
✔️ **Performed Exploratory Data Analysis (EDA)** to discover customer behavior insights.  
✔️ **Created visualizations** using **Matplotlib & Seaborn** for better understanding.  
✔️ **Analyzed key factors such as:**  
   - Most popular product categories.  
   - Revenue trends across states and cities.  
   - Impact of gender and age group on purchasing behavior.  

## 🛠️ Technologies Used  
- **Python**  
- **Pandas** (for data cleaning & analysis)  
- **Matplotlib & Seaborn** (for visualization)  
- **NumPy**  
- **Jupyter Notebook**  

## 📊 Sample Analysis  
### 🔹 1. Most Popular Product Categories  
```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd

# Load dataset
df = pd.read_csv("diwali_sales_data.csv")

# Count product categories
category_counts = df['Category'].value_counts().head(10)

# Plot top categories
plt.figure(figsize=(10,5))
sns.barplot(x=category_counts.index, y=category_counts.values, palette="coolwarm")
plt.title("Top 10 Most Purchased Product Categories")
plt.xlabel("Category")
plt.ylabel("Number of Purchases")
plt.xticks(rotation=45)
plt.show()
