
# Data Analyst Job Market Dashboard & Analysis

## Introduction
This project explores the data analyst and data science job market using Excel, combining an interactive salary dashboard with a deeper analysis of skills, demand, and compensation trends. The goal is to help identify what roles pay the most, which skills are worth learning, and how salary varies by region and experience.

This project is split into two files:
- [**Dashboard**](https://github.com/DeonAqsa/Project_Data_Analysis-Excel/blob/a9939bcb7ffae2afcfd26de659bb74c3c06a3a84/Project%201%20Dashboard.xlsx) — an interactive salary calculator built with Excel formulas (IF, XLOOKUP, IFERROR, etc.)
- [**Analysis Workbook**](https://github.com/DeonAqsa/Project_Data_Analysis-Excel/blob/4b98b48e48e6c49840322b1997b25f16e89abc7e/Project%20Excel%202%20Power%20PIvot%2C%20Queries%2C%20Table.xlsx) — a deeper dive using PivotTables, Power Query, and Power Pivot

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
A calculator-style dashboard where you can filter by **Job Title**, **Country**, and **Schedule Type** to instantly see the median salary, top job platform, and job count for that combination.
   
<img width="*800" alt="Dashboard Records (1) (online-video-cutter com)" src="https://github.com/user-attachments/assets/8875d125-b849-400b-aa3c-5aae72231a06" />

**Insight:** This dashboard allows salary figures to be looked up by specific criteria, simply select a job title, country, and schedule type, and the median salary, job count, and top hiring platform are displayed instantly. It offers a personalized reference instead of relying on general averages.

---

### 2. Salary Comparison
Compares hourly and yearly average salary across job titles.
<img width="2503" height="974" alt="Picture2" src="https://github.com/user-attachments/assets/b112d01a-a5ba-4c58-908a-d4f04464f1c9" />
**Insight:** Senior Data Scientist has the highest average yearly salary at $154,093, while Business Analyst sits at the bottom at $91,217, roughly 40% lower.

---

### 3. Skill's Demand
Counts how often each skill appears across job postings.
<img width="1655" height="989" alt="Picture3" src="https://github.com/user-attachments/assets/a0619a1a-6b97-4209-97e2-e497309806f3" />

**Insight:** SQL and Python dominate demand, together making up nearly 45% of the total 81,948 skill mentions, far ahead of visualization tools like Tableau or R.

---

### 4. Skill's Salary
Compares each skill's demand against its average yearly salary.
<img width="1991" height="1133" alt="Picture4" src="https://github.com/user-attachments/assets/424d880f-16d4-45d4-8705-8ad6e28060f2" />
**Insight:** Spark pays the most on average ($136,092) despite having the lowest demand on this list, while Excel, the most accessible skill, pays the least at $91,956.

---

### 5. Salary per Skills Comparison
Looks at whether having more skills correlates with a higher salary, and how pay differs by region.
<img width="1990" height="1101" alt="Picture5" src="https://github.com/user-attachments/assets/604fff0c-70a4-4e72-af04-b0c9a2e4006e" />
**Insight:** Roles that require more skills per job generally pay more, Senior Data Engineer requires the most skills (8.1) and pays the highest ($147,500) among non-scientist roles. Regionally, salaries in the US are consistently equal to or higher than non-US salaries across every role.

---

### 6. Most Optimal Skill to Learn (Power Pivot)
Combines each skill's likelihood of appearing in a job posting with its median salary to find the best skill to prioritize.
<img width="2323" height="1384" alt="Picture6" src="https://github.com/user-attachments/assets/49f1bb91-ab98-4db9-ad25-d044cef9291e" />
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


