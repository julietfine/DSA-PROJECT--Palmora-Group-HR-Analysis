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

---

### 📎 Files Used  
-- `Palmoria Group emp-data$`  *(add link when uploaded)*
- `Palmoria Group Bonus Rules$`*(add link when uploaded)*
- 

---
