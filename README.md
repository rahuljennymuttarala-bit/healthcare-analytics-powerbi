# Healthcare Analytics Dashboard – Power BI

## 📊 Project Overview

This project is an interactive **Healthcare Analytics Dashboard** developed using **Microsoft Power BI**.

The objective of this project is to analyze healthcare operations and provide meaningful insights into:

- Patient volume
- Medical procedures
- Hospital departments
- Payments and revenue
- Patient encounters
- Average length of stay
- Monthly payment trends
- Department-level performance

The project demonstrates practical skills in **data cleaning, data modeling, DAX, Power BI visualization, and business analysis**.

---

## 🎯 Business Objective

Healthcare organizations generate large amounts of operational and financial data.

This dashboard helps management understand:

- How many patients are being handled?
- Which departments have higher patient activity?
- How many procedures are being performed?
- How are payments distributed across departments?
- How do payments change throughout the year?
- Which departments have higher encounter volumes?
- What is the average patient length of stay?

The dashboard converts raw healthcare data into an interactive reporting solution that can support operational decision-making.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Data source / raw data |
| Power BI Desktop | Dashboard development |
| Power Query | Data cleaning and transformation |
| DAX | Measures and calculations |
| Power BI Data Model | Relationships between tables |
| GitHub | Project documentation and portfolio |

---

## 🗂️ Data Model

The project uses multiple related tables to create a structured healthcare data model.

### Main Tables

- Patients
- Admissions
- Doctors
- Departments
- Encounters
- Procedures
- Billing
- Payments
- DateTable

The model uses relationships between fact and dimension tables to enable cross-filtering and analysis.

### Important Relationships

Examples include:

- Admissions → Patients
- Admissions → Doctors
- Admissions → Departments
- Admissions → DateTable
- Billing → DateTable
- Billing → Payments
- Doctors → Departments
- Encounters → Patients
- Encounters → Doctors
- Encounters → Departments
- Payments → Patients
- Procedures → Departments

---

# 📈 Dashboard

The Power BI report contains **2 dashboard pages**.

## Page 1 – Healthcare Overview

The first dashboard provides a high-level overview of healthcare operations.

Key KPI metrics include:

- **Total Patients:** 10K
- **Total Procedures:** 5K
- **Total Payments:** 24M
- **Average Length of Stay:** 6.47

The page provides management with a quick overview of the overall healthcare operation.

---

## Page 2 – Department & Payment Analysis

The second dashboard focuses on department-level and payment analysis.

### Visualizations

#### 1. Count of Patient_ID by Department_Name

Shows the number of patients associated with each department.

This helps identify departments with higher patient activity.

#### 2. Total Payments by Month Short

A monthly trend visualization showing how total payments change throughout the year.

This helps identify:

- High-payment months
- Low-payment months
- Monthly fluctuations
- Overall payment trends

#### 3. Count of Procedure_ID by Department_Name

Shows the number of procedures performed across departments.

This can help compare procedure activity between departments.

#### 4. Total Payments by Department_Name

Shows total payments associated with each department.

This helps identify departments contributing higher payment volumes.

#### 5. Completed Encounters by Department_Name

Shows completed healthcare encounters by department.

This provides an operational view of department activity.

---

# 📌 Key KPIs

### Total Patients

Measures the total number of patients available in the dataset.

```DAX
Total Patients =
DISTINCTCOUNT(Patients[Patient_ID])
