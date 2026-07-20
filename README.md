<div align="center">

# 💳 Loan Repayment Rate (LRR) Analysis
### End-to-End Exploratory Data Analysis on Consumer Loan Dataset

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?style=for-the-badge&logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?style=for-the-badge)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-green?style=for-the-badge)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Charts-3F4F75?style=for-the-badge&logo=plotly)

**An end-to-end data analytics project that cleans, explores, visualizes, and analyzes loan repayment behavior to uncover insights about credit risk, default patterns, and repayment performance.**

</div>

---

# 📌 Project Overview

Financial institutions rely on historical loan data to understand borrower behavior and reduce lending risks.

This project performs a complete **Exploratory Data Analysis (EDA)** on a consumer loan dataset by:

- Cleaning missing and inconsistent data
- Engineering meaningful financial features
- Detecting and handling outliers
- Visualizing repayment trends
- Performing statistical hypothesis testing
- Extracting actionable business insights

The project introduces a custom metric called **Loan Repayment Rate (LRR)** to evaluate repayment efficiency across different borrower segments.

---

# 🎯 Objectives

- Analyze borrower repayment behavior
- Identify factors affecting loan default
- Compare repayment performance across loan grades
- Study the relationship between debt burden and repayments
- Provide business recommendations for improving lending decisions

---

# 📂 Dataset

The dataset contains consumer loan information including:

- Loan Amount
- Funded Amount
- Interest Rate
- Loan Grade
- Loan Status
- Annual Income
- Debt-to-Income Ratio (DTI)
- Recoveries
- Total Payment
- Loan Purpose
- Delinquencies
- Term

The dataset is automatically downloaded from Google Drive using **gdown**.

---

# 🛠️ Technologies Used

| Category | Tools |
|----------|-------|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Plotly |
| Statistics | SciPy |
| Notebook | Google Colab / Jupyter |

---

# 📊 Workflow

```
Dataset
   │
   ▼
Data Loading
   │
   ▼
Data Cleaning
   │
   ▼
Feature Engineering
   │
   ▼
Outlier Handling
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Statistical Testing
   │
   ▼
Business Insights
```

---

# ⚙️ Data Preprocessing

The following preprocessing steps were performed:

✔ Missing value treatment

✔ Duplicate record detection

✔ Interest rate conversion from percentage to numeric

✔ Loan term conversion into months

✔ Loan Repayment Rate (LRR) feature creation

✔ Default flag generation

✔ Outlier capping using percentile clipping

---

# 📈 Feature Engineering

### Loan Repayment Rate (LRR)

```python
LRR = (Total Payment / Funded Amount) × 100
```

Higher values indicate stronger repayment performance.

---

### Default Flag

```python
is_default = 1 if loan_status == "Charged Off"
```

Used for default analysis and risk segmentation.

---

# 📊 Exploratory Data Analysis

The project includes multiple visualizations such as:

### 📌 Distribution of Loan Repayment Rate

- Histogram
- KDE Curve

---

### 📌 Loan Grade Analysis

- Boxplots
- Interactive Plotly Bar Charts
- Average LRR by Grade

---

### 📌 Default Rate Analysis

- Default Percentage by Grade
- Risk Comparison

---

### 📌 Correlation Analysis

Heatmap of important financial variables including:

- LRR
- Interest Rate
- DTI
- Annual Income
- Loan Amount
- Term
- Delinquencies

---

### 📌 Loan Purpose Analysis

Average repayment performance across different loan purposes.

---

### 📌 Recovery Rate Analysis

Calculated recovery efficiency on defaulted loans.

---

# 📉 Statistical Analysis

The project performs hypothesis testing using an independent **T-Test**.

### Hypothesis

**H₀:** Debt-to-Income Ratio has no impact on Loan Repayment Rate.

**H₁:** Debt-to-Income Ratio significantly affects Loan Repayment Rate.

SciPy is used to calculate the p-value and determine statistical significance.

---

# 📌 Key Insights

### 📉 Loan Grades

Lower credit grades (E–G)

- Higher default rates
- Lower repayment performance

---

### 💰 Debt-to-Income Ratio

Borrowers with higher DTI generally show:

- Lower repayment efficiency
- Increased financial risk

---

### 📈 Interest Rates

Higher-risk borrowers pay higher interest rates, although pricing can still be optimized.

---

### 🔄 Recovery Performance

Recovery rates on defaulted loans suggest opportunities to improve collection strategies.

---

# 💡 Business Recommendations

- Implement smarter risk-based pricing models
- Monitor high-DTI borrowers proactively
- Improve post-default recovery mechanisms
- Build predictive models using behavioral and financial features
- Segment borrowers based on repayment behavior

---

# 📁 Output Files

After execution, the project generates:

```
NL_UCUCI_cleaned.csv
```

Cleaned dataset with engineered features.

```
NL_UCUCI_grade_summary.csv
```

Summary statistics by loan grade including:

- Average LRR
- Loan Count
- Default Rate
- Average Interest Rate

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Loan-Repayment-Analysis.git
```

Install dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly scipy statsmodels gdown
```

Run the notebook or Python script.

---

# 📚 Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- plotly
- scipy
- statsmodels
- gdown

---

# 📌 Future Improvements

- Predictive Machine Learning models
- Loan default prediction
- Credit risk scoring
- Interactive dashboard using Power BI or Streamlit
- Time-series repayment forecasting

---

# 👩‍💻 Author

**Shikha Yadav**

Electrical Engineering Undergraduate  
National Institute of Technology Raipur

Interested in:

- Data Analytics
- Machine Learning
- Business Intelligence
- Financial Data Analysis

---

<div align="center">

### ⭐ If you found this project useful, don't forget to star the repository!

**Happy Coding! 🚀**

</div>
