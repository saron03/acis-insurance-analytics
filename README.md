# ACIS Car Insurance Analytics Project

This repository contains data analysis, statistical testing, and predictive modeling for AlphaCare Insurance Solutions (ACIS). The goal is to identify low-risk customers and help ACIS develop better pricing strategies.

---

## Tasks

- **Task 1:** Git & GitHub Setup + Exploratory Data Analysis (EDA)
- **Task 2:** Data Version Control (DVC)
- **Task 3:** Hypothesis Testing
- **Task 4:** Predictive Modeling

---

## Tools Used

- Python  
- Git & GitHub  
- DVC  
- Pandas, NumPy, Seaborn, Matplotlib  
- Scikit-learn  

---

## Task 1: Git & GitHub + EDA

### 1.1 Git and GitHub

- A GitHub repository was created for the project with proper structure and documentation.
- Branching strategy applied: `main`, `task-1`, `task-2`, etc.
- Multiple commits with descriptive messages have been made for clarity and version tracking.
- A GitHub Actions workflow is set up for CI/CD (optional enhancement).

### 1.2 Exploratory Data Analysis (EDA)

This phase focused on understanding the insurance portfolio data, identifying trends, outliers, and initial signals for risk profiling and pricing strategies.

#### Data Summarization

- Descriptive statistics were generated for key variables:  
  - `TotalPremium`, `TotalClaims`, `CustomValueEstimate`
- Data types and structures were reviewed and cleaned as needed.

#### Data Quality Checks

- Missing values were identified and visualized.
- Columns with formatting issues (e.g., date, category types) were fixed.

#### Univariate Analysis

- Histograms for numeric variables and bar plots for categorical features.
- Outlier detection via box plots on `TotalClaims`, `TotalPremium`, and `CustomValueEstimate`.

#### Bivariate/Multivariate Analysis

- Correlation matrix between key financial metrics.
- Scatter plots: `TotalPremium` vs `TotalClaims`, grouped by `ZipCode`, `Gender`, and `VehicleType`.
- Group-wise Loss Ratio (TotalClaims / TotalPremium) analyzed by:
  - `Province`
  - `Gender`
  - `VehicleType`

#### Trends Over Geography and Time

- Monthly trends over 18 months to detect shifts in frequency and severity.
- Changes in vehicle types and cover types over regions visualized.
- Temporal analysis to detect seasonality or spikes in claim behavior.

#### Highlight Plots

Three creative visualizations were generated to demonstrate key insights:
1. **Loss Ratio by Vehicle Type and Gender**
2. **Monthly Claim Amount Trends**
3. **Boxplot of TotalClaims across Provinces**

---

## Getting Started

To clone and reproduce this project:

```
git clone https://github.com/saron03/acis-insurance-analytics.git
cd acis-insurance-analytics
pip install -r requirements.txt
```