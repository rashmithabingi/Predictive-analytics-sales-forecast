# Predictive-analytics-sales-forecast
"Sales forecasting project using Excel,Python,and Power BI"
# Predictive Analytics Using Historical Data

A sales forecasting project that predicts future retail sales trends using historical data, built with Excel, Python, and Power BI.

## Problem Statement
Retail businesses need to forecast future sales to plan inventory, staffing, and promotions effectively. This project builds a predictive model to estimate daily store sales based on historical patterns, promotions, holidays, and store characteristics.

## Tools Used
- **Excel** – Initial data review and formatting
- **Python** (pandas, scikit-learn, matplotlib) – Data cleaning, feature engineering, model building, and evaluation
- **Power BI** – Interactive dashboard for visualizing actual vs. predicted sales

## Approach
1. **Data Preparation**: Loaded and merged store sales data with store metadata (type, assortment, competition distance)
2. **Feature Engineering**: Extracted Year, Month, Day, and IsWeekend from the date column; removed closed-store records
3. **Model Building**: Trained a Random Forest Regressor to predict daily sales using store, promotion, holiday, and store-type features
4. **Evaluation**: Achieved an RMSE of ~713 and MAE of ~542 on the test set
5. **Visualization**: Built a Power BI dashboard with an actual vs. predicted sales line chart, sales-by-store bar chart, and KPI summary cards

## Key Results
- **RMSE**: 713.42
- **MAE**: 542.47
- Model closely tracks actual sales trends across stores, including seasonal spikes and promotional effects

## Files in This Repository
- `Untitled1.ipynb` – Python notebook with full data cleaning, model training, and evaluation code
- `train.csv`, `store.csv` – Source sales and store data
- `sales_cleaned.xlsx` – Reviewed dataset in Excel
- `predictions_for_powerbi.csv` – Model output used for the dashboard
- `actual_vs_predicted.png` – Chart comparing actual vs. predicted sales
- `sales_dashboard.pbix` – Power BI dashboard file

## Dashboard Preview
See `actual_vs_predicted.png` for a preview of model performance.
