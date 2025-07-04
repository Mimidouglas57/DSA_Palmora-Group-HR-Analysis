# DSA_Palmora-Group-HR-Analysis
This project is part of my DSA training and showcases a complete HR analytics case study for Palmoria Group, a Nigerian manufacturing company. The analysis focuses on performance-based compensation, gender pay gap insights, salary band distribution, and regulatory compliance.

## 📚 Table of Contents

1. [📌 Project Overview](#-project-overview)  
2. [🎯 Objectives](#-objectives)
3. [🧹 Data Cleaning Steps](#-data-cleaning-steps)
4. [🔍 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
5. [🛠 Tools & Techniques](#-tools--techniques)  
6. [📊 Visualizations & Insights](#-visualizations--insights)  
7. [📁 Files Included](#-files-included)  
8. [📝 Recommendations](#-recommendations)  
9. [🏁 Conclusion](#-conclusion)

## 📌 Project Overview

The Palmoria Group HR Analytics Project focuses on analyzing employee compensation, gender equity, and performance-based bonuses to support informed decision-making and ensure regulatory compliance.


## 🎯 Objectives

- Automate annual bonus allocation based on performance
- Evaluate salary fairness across gender, departments, and regions
- Ensure compliance with minimum wage regulations
- Provide actionable insights for HR improvement

## 🧹 Data Cleaning Steps
Initial data exploration focused on cleaning and preparing the employee and bonus datasets for analysis. Key steps included:

- Assigned `"Undisclosed"` to employees who didn’t reveal their gender  
- Removed employees with missing salaries (no longer with the company)  
- Filtered out records with `"NULL"` department entries  
- Replaced blank bonus fields with `0`  
- Verified data types and checked for outliers  
- Ensured performance ratings aligned with bonus rules

These steps ensured a clean, reliable dataset for analyzing salary structures, pay gaps, and bonus allocations.


## 🔍 Exploratory Data Analysis (EDA)
This section presents the initial exploration of Palmoria's HR dataset, focusing on gender representation, performance fairness, salary structure, and compensation equity.

- Gender Distribution
- Performance Ratings by Gender
- Salary Structure & Gender Pay Gap
- Minimum Salary Compliance ($90,000 Regulation)
- Salary Band Distribution
- Bonus & Total Compensation

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


![Gender Distribution by Department](https://github.com/user-attachments/assets/ff522350-6f9a-46b5-9eff-e9103f25f838)



The overall gender distribution across departments is relatively balanced.

- Female-dominant departments: Services, Business Development, Human Resources, and R&D — indicating strong inclusion in several strategic and technical areas.
- Male-dominant departments: Legal, Support, Accounting, and Sales — these may require closer review for potential gender imbalance.

Engineering and Marketing show perfect or near gender parity, which is a positive sign.

A few departments have high counts of undisclosed gender (e.g., Engineering, R&D), which may mask actual bias and should be addressed.

### 2. Ratings Based on Gender

![Ratings by Gender](https://github.com/user-attachments/assets/3b583b03-f890-4fde-8281-ec7409773578)


- Most employees, regardless of gender, were rated as “Average”, showing consistent evaluation standards.
- More females received “Very Good” ratings (44 vs. 32 males), suggesting strong performance or recognition.
- More males were rated “Poor” and “Very Poor” than females, which may indicate performance gaps or stricter assessments in male-dominated roles.
- No clear signs of systemic gender bias, but these trends may warrant further review by role or department.

### 3. Gender Pay Gap Analysis

- By Location

![Average Salary by Gender per Location](https://github.com/user-attachments/assets/a9942d4b-bd19-46d5-8222-79a79f962cfa)

  - Male employees earn more than female employees in all regions, with the gap most noticeable in Abuja (₦2,621).
  - Undisclosed gender group has the highest average salary across all locations, suggesting possible senior or misclassified roles.
  - The pay differences are modest but consistent, indicating a systemic gender pay gap.

- By Department
  
![Average Salary by Gender per Department](https://github.com/user-attachments/assets/4933b933-23cb-4250-9f41-839654495a39)

- Male employees earn more in most departments, with the largest gaps in:
  - Human Resources
  - Services
  - Business Development
  - Support
- Female employees earn more in:
  - Engineering
  - Marketing
  - Training

Undisclosed gender group often has the highest salaries, especially in Accounting and Marketing — suggesting possible senior or misclassified roles.

### 4. Compliance Check

![Salary Compliance Status](https://github.com/user-attachments/assets/47c59bf5-9527-4735-b3fe-29398a924ece)

❌ Palmoria is not compliant with the new regulation.
    
   - Only 275 out of 874 employees (31.5%) meet the required $90,000 minimum salary.
   - 599 employees (68.5%) fall below the threshold.

### 5. Salary Band Distribution

![Salary Band Distribution](https://github.com/user-attachments/assets/d06da0ba-a9e5-43a3-b3c9-10317c291be2)

  - The largest group of employees (190) earn above $100,000, showing a strong top-end salary cluster.
  - The 70k–90k range is the next most populated band, with over 200 employees combined.
  - A significant portion (≈96) earn between 30k–40k, highlighting a lower pay group.
  - The smallest band is $20k–$30k, with only 26 employees.
  - No employees fall into the $10k–$20k range, indicating a baseline salary above that.

- By Location

![Salary Band Distribution by Location](https://github.com/user-attachments/assets/311856aa-9a63-48c9-8e12-65f0063dfb66)

  - Kaduna consistently has higher counts across most salary bands, especially in 100k+, 70k–80k, and 50k–60k bands.
  - Lagos tends to have fewer employees in lower bands, suggesting a slightly more concentrated higher-paying structure.
  - Abuja shows a balanced distribution but has a noticeable number of employees in both high and low salary bands.

### 6. Bonus Allocation & Total Pay Analysis
Bonus percentages were applied based on performance ratings using a reference rule table.

[Palmoria Group Bonus Rules.xlsx](https://github.com/user-attachments/files/21064251/Palmoria.Group.Bonus.Rules.xlsx)

- **Bonus Amount per Employee**
  Using the dax function
  ```
      BonusAmount = 'Palmoria HR Analytics'[Salary] * Related('Palmoria HR Analytics'[Bonus Rating]
  
- **Total Pay (Salary + Bonus)**
```
      TotalPay =  'Palmoria HR Analytics'[Salary] + 'Palmoria HR Analytics'[BonusAmount]
```

- **Total Amount Paid Out by Region**
  ```
      TotalBonusByRegion = SUM('Palmoria HR Analytics'[BonusAmount])
      TotalPayByRegion = SUM('Palmoria HR Analytics'[TotalPay])
``
  - **Company-Wide Total**
    ```
        TotalBonusCompany = SUM('Palmoria HR Analytics'[BonusAmount])
        TotalPayCompany = SUM('Palmoria HR Analytics'[TotalPay])


## 📝 Recommendations



## 📁 Files Included

- `Palmoria_HR_Analytics_Report.pdf`
- `Palmoria_Dashboard.pbix`
- `cleaned data Palmoria Group emp-data.xlsx`
- `Palmoria Group Bonus Rules.xlsx`
