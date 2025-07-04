# DSA_Palmora-Group-HR-Analysis
This project is part of my DSA training and showcases a complete HR analytics case study for Palmoria Group, a Nigerian manufacturing company. The analysis focuses on performance-based compensation, gender pay gap insights, salary band distribution, and regulatory compliance.

## 📚 Table of Contents

1. [📌 Project Overview](#-project-overview)  
2. [🎯 Objectives](#-objectives)
3. [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)  
4. [🔍 Key Analysis Areas](#-key-analysis-areas)  
5. [🛠 Tools & Techniques](#-tools--techniques)  
6. [📊 Visualizations & Insights](#-visualizations--insights)  
7. [📁 Files Included](#-files-included)  
8. [🖼 Sample Dashboard Preview](#-sample-dashboard-preview)  
9. [🏁 Conclusion](#-conclusion)

## 📌 Project Overview

The Palmoria Group HR Analytics Project focuses on analyzing employee compensation, gender equity, and performance-based bonuses to support informed decision-making and ensure regulatory compliance.


## 🎯 Objectives

- Automate annual bonus allocation based on performance
- Evaluate salary fairness across gender, departments, and regions
- Ensure compliance with minimum wage regulations
- Provide actionable insights for HR improvement

## 🔍 Exploratory Data Analysis (EDA)

Initial data exploration focused on cleaning and preparing the employee and bonus datasets for analysis. Key steps included:

- Assigned `"Undisclosed"` to employees who didn’t reveal their gender  
- Removed employees with missing salaries (no longer with the company)  
- Filtered out records with `"NULL"` department entries  
- Replaced blank bonus fields with `0`  
- Verified data types and checked for outliers  
- Ensured performance ratings aligned with bonus rules

These steps ensured a clean, reliable dataset for analyzing salary structures, pay gaps, and bonus allocations.

## 🔍 Key Analysis Areas

- 📈 **Gender Pay Gap Analysis**
- 💰 **Bonus Allocation Based on Performance**
- 🏙 **Salary Band Distribution by Region**
- ✅ **$90,000 Minimum Wage Compliance**
- 📊 **Company-Wide and Regional Payroll Summaries**
  
## 🛠 Tools & Techniques

- **Power BI** – Interactive dashboards & visuals  
- **Power Query** – Data cleaning and transformation  
- **DAX** – Custom metrics and logic (e.g., bonus calculations, pay gap analysis)  
- **Excel** – Business rules and bonus inputs

## 📊 Visualizations & Insights
### Key Findings

### 1. Gender distribution by department, and region 
- Total employees: 874
- Male: 430 (49.2%)
- Female: 406 (46.45%)
- Undisclosed: 38 (4.35%)

The gender split is relatively balanced overall — with males slightly ahead by ~2.75%. This does not suggest strong company-wide gender bias in hiring, but the presence of 4.35% undisclosed cases shows a small gap in data completeness or sensitivity in disclosure.

By Region:
- Kaduna
  - Male: 172
  - Female: 151
  - Undisclosed: 14

Kaduna shows a modest male dominance (53.3% male vs 46.7% female when excluding undisclosed). This could be due to region-specific hiring patterns or job roles that tend to attract more men.

- Abuja
  - Male:144
  - Female: 144
  - Undisclosed: 16

Abuja has perfect gender parity among disclosed employees — a strong sign of balanced hiring. However, 16 people (5.3%) did not disclose their gender, slightly higher than the overall average.

- Lagos:
  - Male: 114
  - Female: 111
  - Undisclosed: 8

Lagos also shows a near-equal gender ratio — suggesting no clear bias. The small undisclosed count (3.4%) shows good data completeness for this region.


By Department

![Gender Distribution by Department](gender-distribution.png)

The overall gender distribution across departments is relatively balanced.

- Female-dominant departments: Services, Business Development, Human Resources, and R&D — indicating strong inclusion in several strategic and technical areas.
- Male-dominant departments: Legal, Support, Accounting, and Sales — these may require closer review for potential gender imbalance.

Engineering and Marketing show perfect or near gender parity, which is a positive sign.

A few departments have high counts of undisclosed gender (e.g., Engineering, R&D), which may mask actual bias and should be addressed.

The gender split is close, but subtle male dominance is seen in all regions.
By Depar
tment: Some departments show skewed gender distribution, particularly in Accounting, Legal, Product Management and Sales, is seen to have more males than female while department like Business development, Engineering, Research and development, Services have more female and others share equal or a little difference in number.



 
- Bonus amount by performance rating  
- Total pay comparison across regions  
- Employees grouped by salary bands  
- KPI cards showing company-wide bonus-to-pay ratio  


## 📁 Files Included

- `Palmoria_HR_Analytics_Report.pdf`
- `Palmoria_Dashboard.pbix`
- `cleaned data Palmoria Group emp-data.xlsx`
- `Palmoria Group Bonus Rules.xlsx`
