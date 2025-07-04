# DSA-PROJECT--Palmora-Group-HR-Analysis
Palmoria Group launches a reform initiative to tackle gender inequality across its regions after recent media backlash. The project targets pay equity, leadership balance, and inclusive culture as it sets sights on ethical global growth.

## 📊 Project Title: Palmoria Group HR Analysis

### 🔍 [Project Overview](#project-overview)

A data-driven HR analysis project focused on uncovering gender-related insights and organizational patterns within the Palmoria Group. Developed as part of a DSA training capstone for capacity building. This project was developed as part of the **DSA Capstone** on data analysis and contributes to my ongoing **upskilling in data analytics**. It focuses on HR data from the Palmoria Group, with an emphasis on workforce analysis, gender representation, and compensation trends.

### 📁 Data Sources  
- Sourced from the DSA Class materials provided for capstone analysis and training.
- `Palmoria Group emp-data$`  
- `Palmoria Group Bonus Rules$`  
These datasets were sourced from the DSA platform’s LMS and provided by the course facilitators.

### 🛠 Tools Used  
- **Microsoft Excel 365** – for preliminary exploration  
- **Microsoft Power BI** – for data cleaning, modeling, and visualization

### 🧹 Data Cleaning & Preparation  
Performed in Power BI using Power Query. Key cleaning steps included:
- Removal of duplicate and incomplete records  
- Employees with **no disclosed gender** were assigned a generic “Undisclosed” status  
- Records for **former employees without salary data** were excluded from analysis  
- Entries with **NULL department values** were also removed  

---
### 🛠 Tools Used  
- [Microsoft Excel](http://www.microsoft.com) – Initial data review and inspection  
- **Power BI** – Data cleaning, visualization, and DAX analysis  
- **Github** – Portfolio building and version control

---

### 🧹 Data Cleaning & Preparation  
Conducted using Power BI and Excel. Key steps included:  
1. Data loading and inspection  
2. Handling missing values and inconsistencies  
3. Data formatting for analysis readiness

---

### 🔍 Exploratory Data Analysis (EDA)  
Key business questions explored during EDA:  
1. What is the gender distribution in the organization? Distil to regions and departments
2. Show insights on ratings based on gender
3. Analyse the company’s salary structure. Identify if there is a gender pay gap. If there is, identify the department and regions that should be the focus of management
4. A recent regulation was adopted which requires manufacturing companies to pay employees a minimum of $90,000
● Does Palmoria meet this requirement?
● Show the pay distribution of employees grouped by a band of $10,000. For example:
● How many employees fall into a band of $10,000 – $20,000, $20,000 – $30,000, etc.?

---
### Data Modelling
The data was modelled and relatioships were created to improve the data analysis. Below is a screenshot of the data model:

![Screenshot 2025-07-04 214528](https://github.com/user-attachments/assets/2f88b29b-c0e6-4eed-860d-03aed991689d)

---

### 📊 Data Visualization  

**Power BI Visual Snapshot**  
![Screenshot 2025-07-04 213809](https://github.com/user-attachments/assets/8054cb6f-bbfb-459e-baf9-c74b1f443741)
![Screenshot 2025-07-04 213833](https://github.com/user-attachments/assets/d03b818a-25d5-4c1d-85fa-9d48e4c586ca)
![Screenshot 2025-07-04 213848](https://github.com/user-attachments/assets/a2f6386e-5e83-4195-bd14-1793dadce72a)
![Screenshot 2025-07-04 213903](https://github.com/user-attachments/assets/5d00fa4d-2b46-4318-bf96-b64ab6022b87)
![Screenshot 2025-07-04 214500](https://github.com/user-attachments/assets/e024241b-7cb6-44fc-b6ab-3ee0ce02d3c0)



_A video walkthrough of the dashboard recording is avaialbe here - 
https://github.com/user-attachments/assets/09b707c9-3d51-431b-9e1b-e5eb3df1b841

---


### 🧠 Data Analysis & DAX Examples  
Sample DAX expressions used in Power BI analysis:

```DAX
-- Total Salary + Bonus
Total Salary + Bonus = SUM('Palmoria Group emp-data'[Salary + Bonus])

-- Calculate Total Compensation
Salary + Bonus = 'Palmoria Group emp-data'[Salary] + 'Palmoria Group emp-data'[Bonuses]

-- Salary Band Classification
Salary Band = SWITCH(TRUE(),
    'Palmoria Group emp-data'[Salary] < 10000, "Less than $10,000",
    'Palmoria Group emp-data'[Salary] <= 20000, "$10,000–$20,000",
    'Palmoria Group emp-data'[Salary] <= 30000, "$21,000–$30,000",
    'Palmoria Group emp-data'[Salary] <= 40000, "$31,000–$40,000",
    'Palmoria Group emp-data'[Salary] <= 50000, "$41,000–$50,000",
    'Palmoria Group emp-data'[Salary] <= 60000, "$51,000–$60,000",
    'Palmoria Group emp-data'[Salary] <= 70000, "$61,000–$70,000",
    'Palmoria Group emp-data'[Salary] <= 80000, "$71,000–$80,000",
    'Palmoria Group emp-data'[Salary] <= 89999, "$81,000–$90,000",
    'Palmoria Group emp-data'[Salary] >= 90000, "$90,000 & Above"
)
```
### INSIGHTS

---

## 📘 Insight Report  
> _“What gets measured gets improved.”_ This section turns HR analytics into clear strategy.

<details>
<summary><strong>🔍 Click to Expand: Turning HR Data Into Action</strong></summary>

<br>

## 📘 *Beyond the Surface: How Gender Inequality Could Stall Palmoria’s Growth*

The numbers are in — and beneath **Palmoria Group’s** strong workforce metrics lies a quiet imbalance that could quietly throttle innovation, trust, and long-term sustainability.

Recent HR data visualizations show a workforce of 946 employees, nearly evenly split on paper: **465 males, 441 females, and 40 undisclosed**. But when you look closer at **gender performance ratings, departmental saturation, and regional spread**, the real story emerges.

---

### ⚠️ Gender-Related Red Flags

#### 1. **Disproportionate Performance Ratings**
Across performance categories — especially *Very Good* and *Good* — male employees significantly outnumber females. This trend appears **regardless of department or region**, suggesting possible:
- Implicit bias in performance evaluation methods  
- Unequal access to projects, mentorship, or training opportunities for women  
- Cultural or systemic barriers discouraging female employees from reaching top-tier ratings

Left unaddressed, this risks creating a **glass ceiling effect** within the organization.

#### 2. **Uneven Departmental Representation**
From the visuals, female representation is noticeably lower in **technical, legal, and product-led functions** — areas often linked to strategic decision-making and innovation. Over time, this can:
- Reinforce gender stereotypes in hiring and role assignment  
- Undermine diverse perspectives in core business strategy  
- Signal to future applicants that Palmoria is not a female-forward employer

#### 3. **Undisclosed Genders — A Symptom of Mistrust?**
With 40 employees choosing not to reveal their gender, Palmoria may be facing an issue of psychological safety. Employees withholding demographic data could point to:
- A lack of inclusion in corporate culture  
- Fear of discrimination or marginalization  
- Gaps in communication about how this data is used and protected

---

### 🔧 Pathways to Progress

Palmoria can turn this insight into impact by initiating thoughtful reforms:

#### ✅ **Revamp Performance Evaluation Framework**
- Introduce anonymized peer-review and multi-rater feedback  
- Align evaluation metrics to clear, documented KPIs  
- Audit recent evaluations for pattern-based bias

#### ✅ **Gender-Inclusive Talent Development**
- Launch leadership pipelines specifically for underrepresented groups  
- Offer sponsorship programs and mentorship matching by gender/department  
- Train managers on recognizing and mitigating unconscious bias

#### ✅ **Boost Transparency and Trust in Data Collection**
- Create campaigns explaining why demographic data is collected and how it supports inclusion  
- Assure employees of anonymity and protection in reporting  
- Include “Prefer not to say” as an explicit, non-punitive option

#### ✅ **Recruitment & Retention Recalibration**
- Set gender representation benchmarks per department  
- Diversify hiring panels and standardize job descriptions to be inclusive  
- Conduct stay interviews to understand retention risks for women and minorities

---

### 🎯 A Gender-Smart Future Is a Scalable Future

For a company on the path to international expansion, **equity isn’t just about compliance—it’s a competitive advantage**. Diverse teams innovate faster, adapt better, and drive sustainable growth. By acknowledging and addressing these gender disparities now, Palmoria has the opportunity to model inclusive excellence for the entire West African manufacturing landscape.

---

### 🔧 Recommendations

- **Revise Evaluation Practices**  
  Adopt multi-rater feedback and manager training to ensure fairness.

- **Build Gender-Equity Pipelines**  
  Launch inclusive mentoring, leadership acceleration, and visibility programs.

- **Foster Transparency in Data Collection**  
  Communicate clearly how demographic data supports equity goals, and offer privacy-conscious options.

- **Balance Hiring Across Departments**  
  Use data-driven benchmarks to guide recruitment, retention, and succession planning.

### 🎯 Why It Matters

With international expansion on the horizon, Palmoria has an opportunity to lead by example. A workforce that reflects fairness and diversity isn’t just more ethical—it’s more effective.

</details>

---
---

### 📎 Files Used  
- [Palmoria Group emp-data$](./Palmoria%20Group%20emp-data.csv) *(Palmoria Group emp-data.csv)*
- [Palmoria Group Bonus Rules$](./Palmoria%20Group%20Bonus%20Rules.xlsx) *(Palmoria Group Bonus Rules.xlsx)*
- 

### 📂 Project Files

- 📊 [Power BI Report – DSA Project: Palmoria HR Analysis.pbix](https://github.com/your-username/your-repo-name/blob/main/DSA%20Project%20-%20Palmoria%20HR%20Analysis.pbix?raw=true)

---
