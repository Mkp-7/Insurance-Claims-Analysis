# Insurance Claims Analysis

This project performs predictive analytics on vehicle insurance claims data. It includes data cleaning, feature engineering, predictive modeling, and visualization of claims risk.

## Project Overview

- **Dataset:** 58,000+ insurance policy records with policyholder, vehicle, and claim information.
- **Objective:** Predict the probability of a claim within 6 months and analyze risk patterns.
- **Tools Used:** SQL Server, R, Power BI.

## Workflow

1. **Data Cleaning and Feature Engineering**
   - Raw CSV files are loaded into SQL Server.
   - Features such as `fuel_type_clean`, `transmission_clean`, and `age` categories were created.

2. **Modeling in R**
   - Logistic Regression and Random Forest models were trained to predict `is_claim`.
   - Random Forest achieved ~94% accuracy.
   - Predicted probabilities were stored as `pred_logit` and `pred_rf`.

3. **Export Predictions**
   - Predicted probabilities were exported to SQL Server for further analysis.

4. **Visualization**
   - Power BI dashboards were created to analyze KPIs:
     - Average predicted claim probability by car segment
     - Fuel type
     - Transmission type
     - Policyholder age

## Folder Structure

- `data/` — Original CSV files
- `sql/` — SQL scripts for table creation, cleaning, and views
- `r/` — R scripts for feature engineering, modeling, and exporting predictions
- `powerbi/` — Power BI dashboard file
- `README.md` — Project description

## How to Run

1. Load CSV data into SQL Server using `create_tables.sql` and `clean_data.sql`.
2. Open R scripts in the `r/` folder to perform feature engineering and run models.
3. Export predictions back to SQL Server using `export_predictions.R`.
4. Open the Power BI file to explore dashboards.
