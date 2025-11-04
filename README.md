# Power-BI-HR-Attrition-Dashboard


# **HR Attrition Dashboard — Power BI**

## 📘 **Project Overview**

This repository contains the **HR Attrition Dashboard** built in **Power BI**.  
The goal of this project is to analyze employee attrition patterns and provide insights into workforce trends such as salary, tenure, job roles, and gender-wise attrition.  
It helps HR teams identify key factors influencing attrition and design strategies for better employee retention.

---

## 🗂️ **Dataset**

* **Source:** [IBM HR Analytics Employee Attrition & Performance Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)  
* **File Used:** `WA_Fn-UseC_-HR-Employee-Attrition.csv`  
* **Format:** CSV  
* **Description:**  
  Contains employee-level information such as demographics, job role, department, salary, years at company, and attrition status.

**Key Columns:**
- **Age**  
- **Gender**  
- **Department**  
- **JobRole**  
- **MonthlyIncome**  
- **YearsAtCompany**  
- **Attrition (Yes/No)**  

---

## 💾 **Repository Structure**

📦 PowerBI-HR-Attrition-Dashboard
┣ 📄 README.md → Project documentation
┣ 📄 HR_Attrition_Dashboard.pbix → Power BI project file
┣ 📄 HR_Attrition_Dashboard.jpg → Dashboard image preview
┣ 📄 WA_Fn-UseC_-HR-Employee-Attrition.csv → Dataset

---

## 🎯 **Dashboard Features**

* **KPIs:**
  - Average Salary  
  - Average Tenure  
  - Attrition Rate (%)  
  - Percentage of Employees Promoted Last Year  

* **Visuals:**
  - Attrition Rate by **Department**  
  - Average Salary by **Job Role**  
  - Attrition Rate % by **Gender**  
  - Slicers for **Gender**, **Age**, and **Job Role**  

---

## 🧹 **Data Cleaning (Power Query Steps)**

1. Removed duplicate rows and null records.  
2. Changed data types for numerical and date fields.  
3. Standardized gender and department values.  
4. Created calculated columns for metrics such as tenure and promotion rate.  

---

## ⚙️ **DAX Measures Used**

Average Salary = AVERAGE('EmployeeData'[MonthlyIncome])
Average Tenure = AVERAGE('EmployeeData'[YearsAtCompany])
Attrition Rate % = DIVIDE(
CALCULATE(COUNTROWS('EmployeeData'), 'EmployeeData'[Attrition] = "Yes"),
COUNTROWS('EmployeeData')
) * 100

---

## 🖼️ **Dashboard Preview**

(![HR Attrition Dashboard]((https://github.com/sanjanagawh9443/Power-BI-HR-Attrition-Dashboard-/blob/main/IMG-20251017-WA0004(1).jpg))

---

## 👩‍💻 **Contributor**

**Sanjana Gawhande**
