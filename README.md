# 💼 Data Jobs Salary Dashboard

## 📌 Introduction  
This interactive dashboard helps job seekers and analysts explore salary trends in the data industry. Users can filter salaries by **job title**, **country**, and **work schedule type**, gaining valuable insights into compensation patterns across various roles and regions.

The project uses real-world data science job listings from 2023, transforming raw data into a clear, interactive, and insightful tool built entirely in Excel.

---

## 📁 File  
**File name:** `projet 1.xlsx`  
Contains the full interactive dashboard, including charts, formulas, and dropdown filters.

---

## 🧠 Skills Demonstrated  
- **Formulas & Functions:** MEDIAN, IF, SEARCH, ISNUMBER, and others  
- **Power Query:** Data cleaning and filtering before analysis  
- **Charts:** Column and bar charts for salary comparison  
- **Data Validation:** Dropdown lists for filtering job titles, countries, and schedule types
-  
![1_Salary_Dashboard_Final_Dashboard](https://github.com/user-attachments/assets/99a52eb5-6c1b-4faa-a86e-851ee2c498ac)

---

## 🗂️ Dataset Overview  
The dataset includes thousands of data science job records with the following fields:  
- 👨‍💼 Job Titles  
- 💰 Average Annual Salary (USD)  
- 🌍 Countries  
- 📅 Schedule Types (e.g., Full-time, Contract, Internship)  

---

## 📊 Dashboard Highlights  

### 🔹 Median Salary by Job Title  
- **Chart Type:** Vertical Column Chart  
- Displays median salaries sorted from highest to lowest, highlighting top-paying roles.  
- **Insight:** Engineering and senior-level positions typically offer higher salaries compared to analyst or entry-level jobs.
![1_Salary_Dashboard_Data_Validation](https://github.com/user-attachments/assets/b9e6bc26-74b5-42e2-aa82-5bbdf93d6b1e)

### 🔹 Job Type Salary Comparison  
- Compares average salaries across schedule types (Full-time, Contractor, Internship).  
- Shows the total number of jobs available per schedule type.  
<img width="942" height="1212" alt="1_Salary_Dashboard_Type" src="https://github.com/user-attachments/assets/fbcbe7c6-d06e-4547-85b3-d731f35b845d" />

---

## 📑 Key Formulas  

**Median Salary Filter by Job Title, Country, and Type:**

```excel
=MEDIAN(
  IF(
    (jobs[job_title_short]=A2)*
    (jobs[job_country]=B2)*
    (ISNUMBER(SEARCH(C2,jobs[job_schedule_type])))*
    (jobs[salary_year_avg]<>0),
    jobs[salary_year_avg]
  )
)
```
- Calculates the median salary based on selected filters  
- Excludes invalid or zero salary values  

---

## 🔍 Power Query Processing
Before analysis, Power Query was used to:  
- Remove null or invalid salary entries  
- Standardize column names  
- Apply initial filters and basic transformations  
<img width="446" height="382" alt="Screenshot 2025-07-23 102118" src="https://github.com/user-attachments/assets/bc1a6478-20a8-46a9-ab79-d20f69588f35" />

---
<img width="416" height="460" alt="Screenshot 2025-07-23 102139" src="https://github.com/user-attachments/assets/cf8bbaea-aa58-45ba-a345-e6a2344b35bd" />

---

## 🧪 Project Focus
This project demonstrates proficiency in data cleaning, visualization, and building interactive dashboards. It delivers accurate insights and clear visuals with a smooth user experience, using only Excel’s native capabilities.
