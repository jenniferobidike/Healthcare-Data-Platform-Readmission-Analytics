# End-to-End Healthcare Data Platform: Readmission Analytics & Prediction

![SQL Server](https://img.shields.io/badge/SQL%20Server-Data%20Analysis-blue)
![Python](https://img.shields.io/badge/Python-Pandas%20%7C%20EDA-teal)
![Power%20BI](https://img.shields.io/badge/Power%20BI-Data%20Visualization-orange)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-success)

This project demonstrates the design of an end-to-end data solution for analysing hospital readmissions. It simulates a modern data platform by ingesting, transforming, and structuring healthcare data into analytical datasets that support reporting, dashboarding, and predictive modelling.

The solution combines data engineering workflows with analytical techniques to uncover key drivers of 30-day hospital readmissions.


## 📌 Project Overview

Built an end-to-end data workflow to process and analyse hospital readmission data, transforming raw healthcare records into structured datasets suitable for analytics and business insights.

The project focuses on:
- Data ingestion and transformation using Python and SQL  
- Structuring data into analysis-ready datasets  
- Performing exploratory and SQL-based analysis  
- Delivering insights through Power BI dashboards  
- Building a predictive model for readmission risk  

## ⚙️ Data Workflow

The solution follows a simplified data engineering pipeline:

### 1. Data Ingestion
- Imported raw healthcare dataset from Kaggle (30,000 patient records)  

### 2. Data Transformation
- Cleaned and standardised data using Python (handling missing values, encoding variables, feature engineering)  
- Applied SQL transformations to validate and structure analytical outputs  

### 3. Analytical Dataset Creation
- Prepared structured datasets to support reporting and dashboarding  
- Enabled consistent metrics for readmission analysis  

### 4. Analytics & Modelling
- Conducted exploratory data analysis (EDA)  
- Built a machine learning model to predict 30-day readmission risk
- 
## 🛠️ Tools & Technologies

- **Python** (Pandas, Matplotlib, Seaborn)  
- **SQL Server** (data transformation and analysis)  
- **Power BI** (interactive dashboards and reporting)  

## 📊 Key Findings

- Overall readmission rate: **12.25%**  
- Length of stay showed limited correlation with readmission risk  
- Discharge destination emerged as the strongest predictor:
  - Rehab: **17.5%**
  - Nursing Facility: **16.85%**
  - Home: **10.04%**

## 📈 Visual Outputs

Exploratory analysis visuals are stored in the `outputs/` folder, including:
- Readmission distribution  
- Readmission rate by discharge destination  
- Readmission rate by diabetes status  

## 🧾 SQL Analysis

SQL Server was used to:
- Validate analytical findings  
- Calculate key metrics for reporting  
- Perform aggregations on readmission rates, length of stay, and clinical factors  

This ensured consistency between analytical outputs and dashboard reporting.

## 🧠 Data Engineering Concepts Demonstrated

- End-to-end data workflow from ingestion to analytics  
- Data transformation using Python and SQL  
- Structuring raw data into clean, analysis-ready datasets  
- Supporting consistent reporting through validated data outputs  
- Integration of data processing with BI tools (Power BI)  

## 🔮 Future Improvements

- Implement scalable pipelines using Azure Data Factory or Databricks  
- Introduce dimensional data modelling (star schema) for reporting  
- Adopt a Lakehouse architecture (Bronze / Silver / Gold layers)  
- Automate data validation and testing processes  


## 📂 Dataset

- Source: Kaggle – Hospital Readmission Prediction  
- Size: 30,000 patient records  
- Target variable: 30-day readmission  

## 📊 Power BI Dashboard

This project includes an interactive Power BI dashboard analysing hospital readmission risk using clinical and operational data.

The dashboard is structured into three key areas:
- **Overview:** High-level readmission metrics and trends  
- **Clinical Insights:** Impact of conditions such as diabetes  
- **Operational Insights:** Discharge destination and hospital-related factors  

### 🔹 Page 1: Executive Overview – Readmission Risk

![Executive Overview](powerbi/powerbi_executive_overview.png)

**Highlights**
- Overall readmission rate: **12.25%**
- Highest risk observed for patients discharged to **Rehab** and **Nursing Facilities**
- Readmissions represent a significant operational and care-quality concern

**Visuals**
- KPI cards (Total Patients, Readmission Rate, Avg LOS)
- Readmission distribution
- Readmission share (donut)
- Readmission rate by discharge destination
- Interactive slicers (Gender, Diabetes, Hypertension)

---

### 🔹 Page 2: Clinical Risk Drivers

![Clinical Risk Drivers](powerbi/powerbi_clinical_risk_drivers.png)

**Highlights**
- Patients with **diabetes** and **hypertension** show higher readmission rates
- Chronic conditions increase post-discharge vulnerability
- BMI shows moderate variation but weaker predictive power

**Visuals**
- Readmission rate by diabetes
- Readmission rate by hypertension
- Readmission rate by BMI

---

### 🔹 Page 3: Patient Segmentation & Root Cause Analysis

![Patient Segmentation](powerbi/powerbi_patient_segmentation.png)

**Highlights**
- **Discharge destination** is the strongest driver of readmission risk
- Risk increases further when combined with chronic conditions
- Decomposition tree reveals how factors interact

**Visuals**
- Decomposition Tree (Readmission Rate → Discharge Destination → Diabetes → Hypertension → Gender)
- Medication burden vs length of stay
- Readmission rate by age

---

## Key Takeaway
This dashboard demonstrates end-to-end analytics capability using **SQL, Python, and Power BI**, with a focus on healthcare insights, risk identification, and data-driven storytelling.
