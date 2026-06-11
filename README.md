# AI Data Science Job Market Analysis

## Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) on an AI and Data Science Job Market dataset containing 50,000 job postings.

The objective of this project is to understand hiring trends, salary patterns, experience requirements, remote work distribution, and other factors influencing the AI/Data Science job market.

The project covers:

- Data Understanding
- Data Cleaning & Preprocessing
- Univariate Analysis
- Bivariate Analysis
- Statistical Hypothesis Testing
- Time-based Analysis
- Feature Engineering
- Business Insight Generation

---

## Dataset Information

### Dataset Size

- Total Records: 50,000
- Total Features: 14 (Original)
- Total Features: 20 (After Feature Engineering)

### Coverage

- Countries: 6
- Industries: 5
- Job Titles: 6
- Company Types: 3

### Main Variables

- Job Title
- Company Type
- Industry
- Country
- City
- Remote Type
- Experience Level
- Minimum Experience Years
- Salary Range (Min & Max)
- Employment Type
- Posted Year

---

## Project Workflow

### Day 1 – Data Understanding

- Loaded dataset
- Explored structure and columns
- Checked data types
- Performed initial observations

Notebook:
- `01_data_overview.ipynb`

---

### Day 2 – Data Cleaning & Preprocessing

- Standardized categorical variables
- Checked missing values
- Removed duplicate records
- Performed outlier analysis using IQR
- Created cleaned dataset

Notebook:
- `02_cleaning_preprocessing.ipynb`

Output:
- `data/interim/cleaned_day2.csv`

---

### Day 3 – Univariate & Bivariate EDA

#### Univariate Analysis

- Salary Distribution
- Job Title Distribution
- Country Distribution

#### Bivariate Analysis

- Salary vs Experience Level
- Salary vs Company Size
- Salary vs Remote Type

#### Correlation Analysis

- Correlation Matrix
- Heatmap Visualization

Notebook:
- `03_univariate_bivariate_eda.ipynb`

---

### Day 4 – Statistical Analysis & Feature Engineering

#### Statistical Tests

##### T-Test

Compared salaries between:

- Remote Jobs
- Onsite Jobs

Result:
- No statistically significant difference found

##### ANOVA

Compared salaries among:

- Remote
- Hybrid
- Onsite

Result:
- No statistically significant difference found

##### Chi-Square Test

Tested association between:

- Experience Level
- Remote Type

Result:
- No significant association detected

#### Time-Based Analysis

- Job posting trends by year

#### Feature Engineering

Created new features:

1. Average Salary
2. Salary Range
3. Experience Category
4. Remote Flag
5. High Salary Job
6. Job Age

Notebook:
- `04_stats_time_features_final_insights.ipynb`

Output:
- `data/processed/final_cleaned_day4.csv`

---

### Day 5 – Final Insights & Documentation

- Generated Top 10 Insights
- Segment Analysis
- Data Quality Review
- Project Conclusions
- README Documentation

Notebook:
- `05_final_insights_readme.ipynb`

---

## Key Findings

### 1. Experience Drives Salary

Salary increases significantly as required experience increases.

### 2. Senior Positions Earn the Most

Senior-level roles consistently offer the highest compensation.

### 3. Strong Salary Correlation

Minimum salary and maximum salary show a very strong positive correlation.

### 4. Remote Work Does Not Guarantee Higher Pay

Remote, Hybrid, and Onsite roles exhibit similar salary distributions.

### 5. Stable Job Demand

AI/Data Science job demand remained relatively stable across the analyzed years.

### 6. Geographic Distribution is Balanced

Job opportunities are fairly evenly distributed across all countries in the dataset.

### 7. Diverse Industry Demand

Demand exists across Healthcare, Finance, Education, and Technology sectors.

### 8. No Significant Salary Difference by Work Arrangement

Statistical tests indicate similar salary levels across Remote, Hybrid, and Onsite jobs.

### 9. Clean Dataset

No missing values, duplicate records, or significant outliers were detected after preprocessing.

### 10. Feature Engineering Improved Analysis

Additional features provided deeper insights into compensation and experience patterns.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- Git
- GitHub

---

## Project Structure

```text
ai-data-science-job-market-analysis/

├── data/
│   ├── raw/
│   ├── interim/
│   └── processed/
│
├── notebooks/
│   ├── 01_data_overview.ipynb
│   ├── 02_cleaning_preprocessing.ipynb
│   ├── 03_univariate_bivariate_eda.ipynb
│   ├── 04_stats_time_features_final_insights.ipynb
│   └── 05_final_insights_readme.ipynb
│
├── reports/
│   └── figures/
│
├── README.md
└── requirements.txt
```

---

## How To Run

Clone the repository:

```bash
git clone <repository-url>
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter lab
```

Run notebooks in the following order:

1. 01_data_overview.ipynb
2. 02_cleaning_preprocessing.ipynb
3. 03_univariate_bivariate_eda.ipynb
4. 04_stats_time_features_final_insights.ipynb
5. 05_final_insights_readme.ipynb

---

## Business Questions Answered

- Does experience influence salary?
- Do remote jobs pay more than onsite jobs?
- Which experience level earns the highest salary?
- Are AI/Data Science jobs increasing over time?
- Which countries have the highest demand?
- Does company size affect salary?
- Is remote work associated with compensation levels?

---

## Project Status

✅ Completed

This project successfully completed the full data analysis lifecycle:

- Data Understanding
- Data Cleaning
- Exploratory Data Analysis
- Statistical Testing
- Feature Engineering
- Insight Generation
- Documentation

---

## Author

Aflah Aflu

AI & Data Science Portfolio Project
