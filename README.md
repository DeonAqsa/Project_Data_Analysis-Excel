# Data Analytics Project
## Salary Dashboard  
Hey checkout my dashboard with link below.  


## Salary Analysis  
Here's for detailed analysis.  
[Analysis](https://github.com/DeonAqsa/Project_Data_Analysis-Excel/blob/4b98b48e48e6c49840322b1997b25f16e89abc7e/Project%20Excel%202%20Power%20PIvot%2C%20Queries%2C%20Table.xlsx)  
<img width="749" height="404" alt="Screenshot 2026-06-08 115548" src="https://github.com/user-attachments/assets/d08a456a-9774-469c-859b-eb65b84e5f60" />  
<img width="608" height="368" alt="Screenshot 2026-06-08 115817" src="https://github.com/user-attachments/assets/e33f0f35-73cf-4480-b07b-c77768c87363" />

# Data Analyst Job Market Dashboard & Analysis

## Introduction
This project explores the data analyst and data science job market using Excel, combining an interactive salary dashboard with a deeper analysis of skills, demand, and compensation trends. The goal is to help identify what roles pay the most, which skills are worth learning, and how salary varies by region and experience.

This project is split into two files:
- **Dashboard** — an interactive salary calculator built with Excel formulas (IF, XLOOKUP, IFERROR, etc.)
- **Analysis Workbook** — a deeper dive using PivotTables, Power Query, and Power Pivot

## Background
Both files use the same dataset, containing real-world job postings across various data roles (Data Analyst, Data Engineer, Data Scientist, and more), along with their salaries, required skills, and locations.

Through this project, I wanted to answer:

1. What salary can I expect for a specific job title, country, and schedule type?
2. How does hourly salary compare to yearly salary across different roles?
3. Which skills are the most in-demand?
4. Which skills pay the most, and how does that compare to how in-demand they are?
5. Does having more skills lead to a higher salary, and how does pay compare across regions?
6. What is the most optimal skill to learn (balancing demand and salary)?

## Tools I Used
- **Microsoft Excel** – core tool for the entire analysis
- **Excel Formulas** – IF, XLOOKUP/VLOOKUP, IFERROR, and other formulas to power the interactive dashboard
- **PivotTables** – to summarize and explore the data across roles, skills, and countries
- **Power Query** – to clean and transform the raw job posting data
- **Power Pivot & DAX** – to build relationships between tables and calculate advanced measures

## The Analysis

### 1. Interactive Salary Dashboard
[A calculator-style dashboard](https://github.com/DeonAqsa/Project_Data_Analysis-Excel/blob/a9939bcb7ffae2afcfd26de659bb74c3c06a3a84/Project%201%20Dashboard.xlsx) where you can filter by **Job Title**, **Country**, and **Schedule Type** to instantly see the median salary, top job platform, and job count for that combination.
   
<img width="*800" alt="Dashboard Records (1) (online-video-cutter com)" src="https://github.com/user-attachments/assets/8875d125-b849-400b-aa3c-5aae72231a06" />

**Insight:** This dashboard allows salary figures to be looked up by specific criteria, simply select a job title, country, and schedule type, and the median salary, job count, and top hiring platform are displayed instantly. It offers a personalized reference instead of relying on general averages.

---

### 2. Salary Comparison (Power Query)
Compares hourly and yearly average salary across job titles.

| Job Title | Hourly Salary AVG/Year | Yearly Salary AVG |
|---|---|---|
| Business Analyst | $89,099 | $91,217 |
| Data Analyst | $79,288 | $93,825 |
| Cloud Engineer | $94,766 | $111,268 |
| Software Engineer | $95,332 | $113,305 |
| Senior Data Analyst | $97,971 | $113,822 |
| Machine Learning Engineer | $100,834 | $126,943 |
| Data Engineer | $118,998 | $130,107 |
| Data Scientist | $102,748 | $135,848 |
| Senior Data Engineer | $130,856 | $146,025 |
| Senior Data Scientist | $112,456 | $154,093 |

**Insight:** Senior Data Scientist has the highest average yearly salary at $154,093, while Business Analyst sits at the bottom at $91,217, roughly 40% lower.

---

### 3. Skill's Demand (Power Query)
Counts how often each skill appears across job postings.

| Skill | Demand Count |
|---|---|
| SQL | 18,500 |
| Python | 17,689 |
| Tableau | 7,043 |
| R | 6,929 |
| AWS | 6,844 |
| Excel | 6,260 |
| Spark | 5,290 |
| Sas | 4,806 |
| Azure | 4,760 |
| Java | 3,827 |

**Insight:** SQL and Python dominate demand, together making up nearly 45% of the total 81,948 skill mentions, far ahead of visualization tools like Tableau or R.

---

### 4. Skills Salary (Power Query)
Compares each skill's demand against its average yearly salary.

| Skill | Skills Demand | Yearly Salary AVG |
|---|---|---|
| Excel | 6,260 | $91,956 |
| Sas | 4,806 | $105,208 |
| Tableau | 7,043 | $110,540 |
| SQL | 18,500 | $118,787 |
| R | 6,929 | $119,092 |
| Azure | 4,760 | $125,554 |
| Python | 17,689 | $125,610 |
| Java | 3,827 | $129,723 |
| Aws | 6,844 | $130,534 |
| Spark | 5,290 | $136,092 |

**Insight:** Spark pays the most on average ($136,092) despite having the lowest demand on this list, while Excel, the most accessible skill, pays the least at $91,956.

---

### 5. Salary per Skills & Regional Comparison (Power Pivot)
Looks at whether having more skills correlates with a higher salary, and how pay differs by region.

| Role | Median Salary | Skills Per Job |
|---|---|---|
| Business Analyst | $85,000 | 3.3 |
| Data Analyst | $90,000 | 3.6 |
| Cloud Engineer | $99,150 | 4.8 |
| Machine Learning Engineer | $107,550 | 5.3 |
| Data Engineer | $125,000 | 7.0 |
| Data Scientist | $127,500 | 4.9 |
| Senior Data Engineer | $147,500 | 8.1 |
| Senior Data Scientist | $155,000 | 5.3 |

**Insight:** Roles that require more skills per job generally pay more, Senior Data Engineer requires the most skills (8.1) and pays the highest ($147,500) among non-scientist roles. Regionally, salaries in the US are consistently equal to or higher than non-US salaries across every role.

---

### 6. Most Optimal Skill to Learn (Power Pivot)
Combines each skill's likelihood of appearing in a job posting with its median salary to find the best skill to prioritize.

| Skill | Skill Likelihood | Median Salary |
|---|---|---|
| SQL | 57% | $120,000 |
| Python | 54% | $125,000 |
| Tableau | 22% | $111,175 |
| R | 21% | $119,550 |
| Aws | 21% | $135,000 |
| Sas | 15% | $110,000 |
| Azure | 15% | $125,000 |
| Spark | 16% | $140,000 |
| Java | 12% | $134,241 |

**Insight:** SQL is the most optimal skill overall, appearing in 57% of job postings while still paying a solid $120,000. Python is a close second, slightly more likely to show up in higher-paying roles at $125,000.

## What I Learned
Working on this project helped me build a wider range of Excel skills, including:
- Writing **formulas** like IF, XLOOKUP/VLOOKUP, and IFERROR to build an interactive, filter-driven dashboard
- Using **PivotTables** to quickly summarize and slice large datasets by role, skill, and country
- Cleaning and transforming raw data using **Power Query**, including shaping tables for analysis
- Building relationships between tables and writing **DAX measures** in **Power Pivot** to calculate metrics like median salary and skill likelihood
- Designing charts (bar, scatter, combo charts) to visually communicate salary and demand trends

## Conclusions

### Key Findings

1. **Interactive Dashboard** — Full-time roles pay noticeably more than other schedule types, with Contractor roles close behind while Temp Work and Internships trail significantly.

2. **Salary Comparison** — Senior Data Scientist has the highest average yearly salary at $154,093, while Business Analyst sits at the bottom at $91,217, roughly 40% lower.

3. **Skill's Demand** — SQL and Python dominate demand, together making up nearly 45% of all skill mentions, far ahead of visualization tools like Tableau or R.

4. **Skills Salary** — Spark pays the most on average ($136,092) despite having the lowest demand on the list, while Excel, the most accessible skill, pays the least.

5. **Salary per Skills & Region** — Roles that require more skills per job generally pay more, and salaries in the US are consistently equal to or higher than non-US salaries across every role.

6. **Most Optimal Skill** — SQL is the most optimal skill overall, appearing in 57% of job postings while still paying a solid $120,000, with Python close behind at $125,000.

### Closing Thoughts
This project strengthened my Excel skills across formulas, PivotTables, Power Query, and Power Pivot, and gave me a much clearer picture of how skills, demand, and salary connect in the data job market. Building both an interactive dashboard and a deeper analytical workbook showed me two different ways to turn the same dataset into something useful, one for quick exploration, and one for deeper insight. Moving forward, I plan to keep prioritizing skills like SQL and Python that balance high demand with strong pay, while staying open to specialized tools like Spark that offer a smaller but higher-paying niche.


