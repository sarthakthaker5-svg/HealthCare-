# 🏥 Healthcare Analytics Dashboard

<img src="https://img.shields.io/badge/Power_BI-Data_Visualization-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
<img src="https://img.shields.io/badge/Power_Query-Data_Transformation-2673B8?style=for-the-badge" alt="Power Query">
<img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge" alt="Status: Completed">
<img src="https://img.shields.io/badge/Dataset-55,500_Records-CC0000?style=for-the-badge" alt="Dataset">
<img src="https://img.shields.io/badge/Project-Healthcare_Analytics-1E8449?style=for-the-badge" alt="Healthcare Analytics">

<br>
<img src="https://readme-typing-svg.demolab.com?font=Poppins&weight=600&size=28&duration=3000&pause=1000&color=CC0000&center=true&vCenter=true&width=700&lines=Healthcare+Analytics+Dashboard;Power+BI+Data+Visualization;Patient+%26+Admission+Analysis;Hospital+Billing+%26+Insurance+Insights" alt="Typing SVG for Healthcare Analytics Dashboard" />
<br>

*An interactive Power BI report for exploring patient demographics, hospital admissions, medical conditions, billing, insurance providers, and healthcare trends.*

</div>

---

## 📖 Project Overview

The **Healthcare Analytics Dashboard** is a Power BI data analytics project developed using a healthcare dataset containing **55,500 patient records**.

The project focuses on transforming raw healthcare data into meaningful business insights using Power Query, data modeling, calculated columns, grouped summary tables, filters, slicers, and interactive visualizations.

The report contains four pages: a Home Page, Hospital Patient Analytics Dashboard, Patient Detail, and Billing Analysis. Together, these pages provide an overview of healthcare data, detailed patient records, and billing performance across medical conditions, hospitals, insurance providers, and departments.

---

# 🎥 Project Demo Video

<p align="center">

<a href="https://drive.google.com/file/d/12r8hqstBujHmYa4E45hftWPfpOQCPZAV/view" target="_blank">

<img src="https://img.shields.io/badge/▶️%20Watch%20Project%20Demo-4285F4?style=for-the-badge&logo=google-drive&logoColor=white"/>

</a>

</p>

> 📺 Click the button above to watch the complete project demonstration and SQL explanation video.
---

## 🎯 Project Objectives

- Import and explore the healthcare dataset using Power BI.
- Perform data profiling and quality checks in Power Query.
- Clean and transform patient, hospital, billing, and admission data.
- Create calculated columns for patient age groups, billing tiers, length of stay, and risk classification.
- Build summary tables for medical conditions, hospitals, insurance providers, and monthly admissions.
- Merge healthcare department lookup data with the main dataset.
- Apply parameters, filters, and data preparation techniques.
- Create interactive KPI cards, charts, tables, matrices, and slicers.
- Analyze patient admissions, billing revenue, insurance claims, and healthcare department performance.
- Design a consistent, professional, multi-page Power BI report.

---

## 🛠️ Technologies Used

| Tool / Technology | Purpose |
|---|---|
| Power BI Desktop | Interactive reports and data visualization |
| Power Query Editor | Data cleaning, transformation, merging, appending, and grouping |
| Healthcare Dataset | Main source of patient and hospital data |
| CSV Files | Dataset and department lookup data |
| DAX / Power BI Aggregations | KPI calculations and visual summaries |
| GitHub | Project documentation and version control |

---

## 🗃️ Dataset

| Item | Details |
|---|---|
| Dataset | Healthcare Dataset |
| Number of Records | 55,500 patient records |
| Number of Original Columns | 15 |
| Main Data | Patient demographics, medical conditions, hospital information, admissions, billing, insurance, and test results |
| Lookup Data | Medical condition-to-department mapping |
| Data Preparation Tool | Power Query Editor |
| Reporting Tool | Microsoft Power BI Desktop |

### Main Dataset Fields

The original dataset includes fields related to:

- Name
- Age
- Gender
- Blood Type
- Medical Condition
- Date of Admission
- Doctor
- Hospital
- Insurance Provider
- Billing Amount
- Room Number
- Admission Type
- Discharge Date
- Medication
- Test Results

The department lookup file maps medical conditions to their corresponding departments.

| Medical Condition | Department |
|---|---|
| Cancer | Oncology |
| Diabetes | Endocrinology |
| Hypertension | Cardiology |
| Obesity | Bariatrics |
| Asthma | Pulmonology |
| Arthritis | Rheumatology |

---

## ⚙️ Data Preparation and Power Query

Power Query was used to prepare the dataset before creating the dashboard.

### Data Cleaning and Transformation

The main transformations include:

1. Importing the healthcare dataset and department lookup CSV files.
2. Enabling Column Quality, Column Distribution, and Column Profile for data inspection.
3. Cleaning patient names and doctor names using appropriate text transformations.
4. Converting hospital names to uppercase.
5. Handling negative billing amounts using the absolute value transformation.
6. Rounding billing amounts to create a separate billing column.
7. Converting admission and discharge dates to the Date data type.
8. Extracting admission year, month, and month number.
9. Calculating the length of stay in days.
10. Creating a Patient_ID index starting from 1.
11. Creating conditional columns for Age_Category, Billing_Tier, Stay_Category, and Risk_Flag.

### Conditional Classification

| Column | Classification Logic |
|---|---|
| Age_Category | Senior, Adult, Minor |
| Billing_Tier | Platinum, Gold, Silver, Standard |
| Stay_Category | Long Stay, Medium Stay, Short Stay, Day Case |
| Risk_Flag | High Risk, Monitor, Low Risk |

### Summary Tables

Reference queries and grouping operations are used to prepare the following analytical tables:

- **Condition_Summary:** Patient count, average billing, and average length of stay by medical condition.
- **Hospital_Summary:** Total patients, total billing revenue, and average billing by hospital.
- **Insurance_Summary:** Covered patients, total claims, and average claim by insurance provider.
- **Monthly_Admissions:** Monthly patient counts and billing revenue by admission year and month.

### Additional Power Query Tasks

- Merging the department lookup table with the main healthcare dataset using a Left Outer Join.
- Creating condition and admission-type analysis using pivoting and unpivoting.
- Splitting records by admission year and appending the resulting queries.
- Demonstrating folder-based data import.
- Configuring the MinAge and AdmissionType parameters.
- Reviewing Applied Steps and verifying data types before loading the data into Power BI.

---

## ✨ Dashboard Features

### 🏠 Home Page

- Professional healthcare analytics cover page.
- Three navigation-style sections: Patient Overview, Billing Analysis, and Patient Details.
- Dark navy background with white typography and red accents.
- Healthcare-themed analytics visuals and a consistent corporate design.

### 📊 Page 1 — Hospital Patient Analytics Dashboard

The main dashboard provides an executive overview of healthcare data.

**KPI Cards**

- Total Patients
- Total Billing
- Average Billing per Patient
- Average Length of Stay (Days)

**Charts and Visualizations**

- Patients by Medical Condition — Clustered Bar Chart.
- Top 10 Hospitals by Total Billing Revenue — Clustered Bar Chart.
- Monthly Patient Admissions by Year — Line Chart.
- Insurance Mix — Donut Chart.

**Interactive Features**

- Admission Type tile slicer.
- Medical Condition dropdown slicer.
- Admission Year range slicer.
- Page-level Age_Category filter to exclude Minor by default.
- Visual-level filters for the Top 10 hospitals and valid monthly admissions.
- Interactive filtering between the report visuals.

### 📋 Page 2 — Patient Detail

This page provides a detailed view of individual patient records.

**Patient Details Table**

- Name
- Age
- Age_Category
- Gender
- Medical Condition
- Department
- Admission Type
- Stay_Category
- Length_of_Stay_Days
- Billing_Rounded
- Insurance Provider
- Test Results
- Risk_Flag

**Interactive Features**

- Medical Condition slicer.
- Admission Type slicer.
- Wrapped table text and consistent formatting for readability.

### 💳 Page 3 — Billing Analysis

This page focuses on billing performance and comparisons across departments, medical conditions, and insurance providers.

**Visualizations**

- **Average Billing by Department:** Clustered Column Chart with Billing_Tier as the legend.
- **Billing Matrix:** Medical Condition as rows, Insurance Provider as columns, and total Billing_Amount_Fixed as values.

**Interactive Features**

- Admission Year slicer.
- Comparisons of billing amounts across medical conditions and insurance providers.
- Department-level billing analysis by billing tier.

---

## 🎨 Dashboard Design and Formatting

The report uses a consistent visual theme to create a professional healthcare analytics interface.

| Design Element | Specification |
|---|---|
| Report Layout | 16:9 widescreen |
| Page Background | `#F5F5F5` |
| Primary Accent | `#CC0000` |
| Heading / KPI Text | `#4A4A4A` |
| Secondary Text | `#6B7280` |
| Visual Background | White |
| Visual Borders | Light grey |
| Chart Titles | 12 pt, bold |
| KPI Values | 28 pt, bold |
| Data Labels | 10 pt |
| Header Title | 18 pt, bold |

The design emphasizes clear data presentation, consistent alignment, readable charts, and coordinated formatting across the report pages.

---

## 📸 Report Screenshots

 ## Home Page

<p align="center">
  <img src="Home Page.png" width="900" alt="Home Page">
</p>

---
 <div align="center">

## Hospital Patient Dashboard

<p align="center">
  <img src="Hospital Patient Dashboard.png" width="900" alt="Hospital Patient Dashboard">
</p>

---
 <div align="center">

 ## Patient Detail

<p align="center">
  <img src="Patient Detail.png" width="900" alt="Patient Detail">
</p>

---
 <div align="center">

 ## Billing Analysis

<p align="center">
  <img src="Billing Analysis.png" width="900" alt="Billing Analysis">
</p>

---
 <div align="center">

---

## 🚀 How to Open the Report

1. Install **Microsoft Power BI Desktop**.
2. Download or clone this GitHub repository.
3. Open the `.pbix` Power BI report file.
4. If Power BI cannot locate the source CSV files, select **Transform data → Data source settings** and update the source paths.
5. Select **Close & Apply** if source changes require it.
6. Navigate between the Home Page, Hospital Patient Analytics Dashboard, Patient Detail, and Billing Analysis pages.
7. Use the slicers and filters to explore the data.
8. Select chart elements to test the configured visual interactions.

---

## 🎓 Learning Outcomes

Through this project, I practiced:

- Importing and profiling real-world-style healthcare data.
- Cleaning and transforming data with Power Query.
- Creating conditional columns and calculated data fields.
- Merging lookup data and appending queries.
- Grouping data to create analytical summary tables.
- Working with Power Query parameters and filters.
- Building KPI cards and selecting suitable aggregations.
- Creating bar charts, line charts, donut charts, tables, and matrices.
- Configuring slicers and interactive visual filtering.
- Designing a professional multi-page Power BI report.
- Documenting a data analytics project for a portfolio.

---

## 👨‍💻 Author

**Sarth Thakar**
