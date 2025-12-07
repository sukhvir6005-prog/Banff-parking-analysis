# Banff Parking Analysis & Explainable AI (XAI) + Streamlit App

This repository contains data analysis, explainability work, and an interactive Streamlit web application developed for the Banff Parking Occupancy Prediction project in **CMPT 3835: Work Integrated Learning II**. The app allows users to explore parking behaviour and interpret model predictions using transparent machine learning methods.



#  Project Objectives
- Analyze hourly parking trends across Banff parking units.
- Engineer temporal features to predict occupancy and fullness.
- Build **explainable ML models (XGBoost + SHAP)**.
- Deploy an **interactive Streamlit dashboard** to:
  - Visualize parking trends.
  - Predict fullness (`Is_Full`) and occupancy.
  - Interpret predictions using feature importance.



# Key Insights from Analysis
✔ Parking demand peaks between **11 AM and 3 PM**  
✔ Weekends show **30–40% higher occupancy**  
✔ Central lots (e.g., *Buffalo & Banff*) fill the fastest  
✔ SHAP shows weather has minor influence compared to demand history  
✔ **Top predictive features:**
- `Occupancy_1hr_Ago`
- `Occupancy_24hr_Ago`
- `Capacity`



##  Explainable AI Methods Used
| XAI Tool | Purpose |
|----------|---------|
| **SHAP Summary Plot** | Shows global feature influence |
| **SHAP Bar Plot** | Ranks predictors by importance |
| **SHAP Local (Waterfall)** | Explains individual predictions |
| **Feature Importance Charts** | Validates model logic |



##  Streamlit Application
An interactive dashboard was built using **Streamlit** that enables:
- **Real-time prediction** of whether a parking unit will be full.
- **Dynamic filtering** by:
  - Hour
  - Day
  - Lot name
  - Weekend/Weekday
- **Interactive visualizations**:
  - EDA trend charts
  - Lot capacity comparison
  - Time-based congestion behaviour
- **Explanation panel using SHAP & feature importance** to show *why* a lot was predicted full.

>  *The application layout follows real industry dashboards used by municipalities for traffic monitoring.*


# Repository Contents
| File/Folder | Description |
|-------------|-------------|
| `screenshots/` | EDA charts, SHAP outputs, dashboard preview |
| `streamlit_app/` *(optional)* | Streamlit UI files |
| `notebooks/` *(optional)* | XAI + modelling notebooks |
| `resources/` *(optional)* | Documentation files |

> To protect academic integrity and licences, raw data is not included.



##  Potential Future Improvements
- Integrating **live parking feeds or APIs**
- Adding **event & holiday effects**
- Deploying the model on **Cloud (GCP) with CI/CD**
- Using **Snowflake or BigQuery** for scalable storage


# Author
**Sukhvir Kaur**  
Student ID: *3107537*  
Course: CMPT 3835 – Work Integrated Learning II  
Term: Fall 2025



# Acknowledgements
Instructors: **Uchenna Mgbaja, Palwasha Afsar**  
This project follows **responsible and explainable machine learning practices**, aligned with industry MLOps standards.

