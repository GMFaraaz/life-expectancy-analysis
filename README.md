# 🌍 Life Expectancy Analysis

### 🧠 Project Overview
This project explores global **life expectancy trends** using data from the **World Health Organization (WHO)**.  
We analyze how various social, economic, and health factors — such as GDP, schooling, and healthcare expenditure — impact life expectancy across countries.  
The goal is to uncover insights that can help understand **why some countries live longer than others** and what improvements could lead to longer, healthier lives.

---

### 📊 Dataset Information
- **Dataset Name:** Life Expectancy Data  
- **Source:** WHO via Kaggle  
- **File:** `Life Expectancy Data.csv`  
- **Rows:** 2938  
- **Columns:** 22  
- **Features:** Country, Year, Status (Developed/Developing), Life Expectancy, GDP, BMI, Schooling, Alcohol, and more.  

---

### 🧹 Data Preprocessing
Before analysis, the dataset was cleaned and verified.  
Here’s what we did — and what we decided **not** to do (and why):

| Step | Action | Reason |
|------|---------|--------|
| Missing Values | Checked using `df.isnull().sum()` | To identify incomplete records |
| Duplicates | Checked with `df.duplicated()` | To ensure no data repetition |
| Data Imputation | **Not performed** | Some missing data may represent real-world gaps (e.g., undeveloped healthcare systems) |
| Data Types | Verified with `df.info()` | Ensured numeric columns were correctly typed |
| Outliers | Examined using boxplots | Outliers retained as they represent real variations |

---

### 🔍 Exploratory Data Analysis (EDA)
The notebook covers:
1. General structure exploration (`df.shape`, `df.describe()`)
2. Country and year-wise comparisons
3. Correlation between GDP, schooling, and life expectancy
4. Visualizations:
   - Correlation Heatmap
   - GDP vs Life Expectancy Scatter Plot
   - Schooling vs Life Expectancy Regression Plot
   - Boxplot (Developed vs Developing)
   - Life Expectancy Over Time (Line Plot)

---

### 💡 Key Insights
- **Higher GDP and better education** are strongly correlated with higher life expectancy.  
- **Developed nations** maintain consistent growth and higher averages across decades.  
- **Developing countries** show larger variation due to unstable healthcare and income levels.  
- The **gap between developed and developing countries** narrows over time — a sign of gradual improvement.  

---

### 📂 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/GMFaraaz/life-expectancy-analysis.git
