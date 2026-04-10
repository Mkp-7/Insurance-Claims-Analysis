# Insurance Analytics Projects

This repository contains two independent projects focused on insurance claims analysis using different datasets and approaches.

---

## Project 1: Claims Dashboard

**Folder:** `Claims Dashboard/`  
**Files:**  
- Insurance_Claims_Analysis.pbix  
- claims_data.csv  
- Guide.md
  
### Overview
Power BI dashboard built on a dataset of 1000 insurance claims to analyze patterns in customer profiles, incidents, and vehicle characteristics.

### Key Analysis
- Claims distribution by incident type, severity, and time
- Customer segmentation by age, gender, and occupation
- Vehicle-level analysis (make, model, age)
- Fraud pattern exploration based on available indicators

### Output
- Interactive Power BI dashboard with multiple pages
- KPI-based analysis for claims and customer behavior

---

## Project 2: Predictive Analysis

**Folder:** `Predictive Analysis/`  
**Files:**  
- train.csv  
- test.csv  
- SQL scripts (data cleaning & transformation)  
- R scripts (analysis & modeling)  
- Statistical analysis plots (from R)  

### Overview
End-to-end workflow on 58,000+ insurance policy records covering data cleaning, statistical analysis, and predictive modeling to estimate claim probability.

---

### Workflow

#### 1. Data Preparation (SQL Server)
- Imported raw data into SQL Server
- Cleaned missing values and created derived columns:
  - `fuel_type_clean`
  - `transmission_clean`
- Structured dataset for modeling

#### 2. Statistical Analysis (R)
- Explored distributions of key variables:
  - Policyholder age
  - Car age
  - Segment and fuel type
- Generated plots to understand relationships with claim occurrence

Statistical plots are included in this folder.

#### 3. Predictive Modeling (R)
- Built models to predict `is_claim`:
  - Logistic Regression
  - Random Forest
- Generated probability scores:
  - `pred_logit`
  - `pred_rf`

#### 4. Output Analysis
- Used predicted probabilities to examine:
  - Claim likelihood across segments
  - Differences by fuel type and transmission
  - Patterns across car age and policyholder age

---

## Notes
- The dashboard  focuses on descriptive analytics.
- The predictive model focuses on data processing and modeling.

---

## Tools Used

- SQL Server
- R (randomForest, glm)
- Power BI

---

## Summary

- Claims Dashboard → Business intelligence and visualization  
- Predictive Analysis → Data processing and predictive modeling  
