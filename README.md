# Palmoria_Capstone_Project_Analysis

# 🧑‍💼 Capstone Project: Gender-Based Workforce & Compensation Analysis in Palmoria Manufacturing Company 

## 📊 Project Overview

This analysis explores gender-related dynamics within Palmoria Manufacturing, focusing on **workforce distribution**, **salary structure**, **employee ratings**, and **bonus allocation**. The objective is to uncover any existing gender disparities, compliance with minimum wage regulations, and regional compensation trends, while delivering actionable insights to inform organizational policy and strategic HR decision-making.

---

##  Data Cleaning & Preparation

Prior to analysis, the following data preprocessing steps were executed:

## 🔧 Data Preparation & Transformation Steps

 **Tool Used** 
 
 PowerBI 

### 📁 Datasets Used

- **Palmoria Group Employee Data (`emp-data.csv`)**

- **Palmoria Group Bonus Rules (`bonus-rules.xlsx`)**

### 🧹 Data Cleaning & Preprocessing
- **Excluded records** with:
  - `NULL` values in the **Department** column
  - Missing **Salary** values (representing employees no longer with the company)
- **Reclassified** employees who did not disclose their gender under a generic `"Unspecified"` category to promote inclusivity.

### 🔄 Data Transformation in Power BI
- Imported the **Bonus Rules dataset** into Power BI and used **Unpivot Columns** in Power Query to restructure the bonus data by department and performance rating.

- **Merged Datasets**:
  - Created a **new merged query** to combine the employee data with the bonus rules.
  - Established relationships using **Department** and **Performance Rating** columns to link bonus percentages with each employee.

### 🧮 Calculated Fields
- Created a **Custom Column** to calculate the **Bonus Amount** for each employee:

  ```powerbi
  Bonus = Salary * Bonus Percentage
---

## 📌 Key Findings & Insights

### 1. 🧍‍♂️🧍‍♀️ Gender Distribution

**Organization-wide** gender distribution:
- **Male:** 467 employees (49.4%)
- **Female:** 441 employees (46.6%)
- **Unspecified:** 40 employees (4%)

📍 **By Region**:
- **Kaduna:** Male – 182 | Female – 165 | Unspecified – 14
- **Abuja:** Male – 159 | Female – 158 | Unspecified – 18
- **Lagos:** Male – 124 | Female – 118 | Unspecified – 8

---

### 2. ⭐ Employee Ratings by Gender

**Performance rating patterns reveal:**

| Rating         | Male | Female | Unspecified |
|----------------|------|--------|-------------|
| Average        | 212  | 190    | 18          |
| Good           | 82   | 89     | 0           |
| Very Good      | 36   | 49     | 5           |
| Poor           | 70   | 58     | 3           |
| Very Poor      | 31   | 20     | 3           |
| Not Rated      | 34   | 35     | 2           |


🔎 **Observation**:
- **Female employees received more "Very Good" ratings** than males.
- A **slightly higher concentration of males in "Poor" and "Very Poor"** categories may point to performance discrepancies that warrant further evaluation.

---

### 3. 💰 Salary Analysis & Gender Pay Gap

#### 🧾 General Salary Insights:
- **Minimum salary:** $28,130  
- **Maximum salary:** $119,930  
- **Employees earning above $90,000:** 292  
- **Employees earning below $90,000:** 654  

#### 🚻 Gender Pay Comparison by Region:

| Region | Gender       | Total Salary ($) |
|--------|--------------|------------------|
| Abuja  | Male         | 11,646,040       |
| Abuja  | Female       | 11,131,420       |
| Abuja  | Unspecified  | 1,338,830        |
| Kaduna | Male         | 13,622,690       |
| Kaduna | Female       | 11,929,130       |
| Kaduna | Unspecified  | 1,101,000        |
| Lagos  | Male         | 9,508,400        |
| Lagos  | Female       | 8,751,290        |
| Lagos  | Unspecified  | 694,880          |


🟨 **Insight**:
- A **mild gender pay gap exists**, with male employees consistently earning more across all regions.
- **Kaduna** shows the **largest absolute difference** in male vs. female compensation.
- **Palmoria is non-compliant with the $90,000 minimum salary regulation**, as **over 69% (654 employees)** earn below the threshold.

---

### 4. 📊 Salary Distribution by Bands

**Grouped by $10,000 salary bands**, the distribution reveals:

| Band ($)          | No. of Employees |
|-------------------|------------------|
| $10,000 - $20,000 | XX               |
| $20,000 - $30,000 | XX               |
| $30,000 - $40,000 | XX               |
| ...               | ...              |
| $100,000+         | XX               |

🟨 **Insight**:
- The **majority of employees fall below $90,000**, indicating a potential compliance and morale issue, especially under recent legal regulations.

---

### 5. 🎁 Bonus Allocation Insights

**Total bonus by region**:
- Kaduna: **$825,907**
- Abuja: **$801,149**
- Lagos: **$572,217**

**Bonus Allocation by Gender and Region**:

| Region | Gender      | Bonus ($) | % Share |
|--------|-------------|-----------|---------|
| Kaduna | Female      | 375,238   | 5.10%   |
| Kaduna | Male        | 406,545   | 5.52%   |
| Abuja  | Female      | 397,933   | 5.54%   |
| Abuja  | Male        | 363,271   | 5.00%   |
| Lagos  | Female      | 290,430   | 3.93%   |
| Lagos  | Male        | 259,448   | 3.32%   |

🟨 **Insight**:
- **Female employees received slightly more bonus on average in Abuja and Kaduna**, aligning with their "Very Good" performance ratings.
- **Lagos region lags in both bonus allocation and average performance**, signaling a possible issue with motivation or workforce management.

---

## ✅ Recommendations

1. **Close the gender pay gap**:
   - Conduct salary benchmarking and internal equity audits.
   - Adjust pay in high-gap regions like **Kaduna** and **Lagos**.

2. **Boost compliance with $90,000 salary regulation**:
   - Consider upskilling or reclassifying lower-paid roles.
   - Phase in a salary review plan for sub-threshold employees.

3. **Capitalize on high-performing female talent**:
   - Develop leadership pathways tailored to top-rated female employees.
   - Promote inclusive management strategies.

4. **Improve Lagos region compensation strategy**:
   - Investigate causes for lower bonuses and pay.
   - Align performance management and incentive systems.

---

## 📌 Summary

- Palmoria Manufacturing employs **946 staff**, with **a balanced gender representation**.
- **Slight gender-based performance and pay disparities exist**, especially in Kaduna.
- **Majority (69%) of employees earn below $90,000**, conflicting with new wage policy.
- **Bonus distributions generally reflect employee performance**, with **female employees slightly outperforming** in key regions.

---

## 🏁 Conclusion

The analysis provides actionable insights into Palmoria’s workforce composition, compensation equity, and performance-linked bonuses. By **addressing gender disparities**, **ensuring compliance**, and **leveraging high-performing regions and demographics**, Palmoria can align better with evolving labor regulations and corporate responsibility goals.

---

| Region | Gender      | Bonus ($) | % Share |
|--------|-------------|-----------|---------|
| Kaduna | Female      | 375,238   | 5.10%   |
| Kaduna | Male        | 406,545   | 5.52%   |
| Abuja  | Female      | 397,933   | 5.54%   |
| Abuja  | Male        | 363,271   | 5.00%   |
| Lagos  | Female      | 290,430   | 3.93%   |
| Lagos  | Male        | 259,448   | 3.32%   |


🟨 **Insight**:
- **Female employees received slightly more bonus on average in Abuja and Kaduna**, aligning with their "Very Good" performance ratings.
- **Lagos region lags in both bonus allocation and average performance**, signaling a possible issue with motivation or workforce management.

 
