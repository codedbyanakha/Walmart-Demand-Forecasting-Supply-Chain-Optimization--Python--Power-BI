# Walmart Sales Forecasting (Python + Power BI)

This project focuses on forecasting Walmart’s weekly sales using a machine learning pipeline in Python and interactive visualization in Power BI.
Four datasets — train.csv, features.csv, stores.csv, and test.csv — were merged and cleaned. Missing values were handled, lag and rolling features were engineered, and categorical variables encoded.
A Gradient Boosting Regressor model was trained to predict sales, and the predictions were saved as walmart_forecasts.csv. Two dashboards — Forecast Performance and Store & Category Insights — were built in Power BI to visualize business and forecasting metrics.

🧠 Business Problem

Challenge: Walmart needed accurate demand forecasts to optimize inventory and reduce stock imbalances.
Approach: Built ML-based demand forecasting using historical sales, holidays, CPI, temperature, and unemployment data.
Impact: Improved forecast accuracy and decision-making in supply chain and demand planning.
Lesson: Forecasting integrates data science and BI — crucial for data-driven retail strategies.

⚙️ Approach

1. Data Integration:
Combined train.csv, features.csv, stores.csv, and test.csv into one consolidated dataset for analysis.
2. Data Cleaning & Preparation:
Handled missing values in Markdown, CPI, Fuel_Price, and Temperature, and standardized formats.
3. Feature Engineering:
Created lag features (1, 2, 3, 4, 8, 52 weeks) and rolling averages (3, 4, 8 weeks) to capture seasonality and trend patterns.
4. Model Development:
Trained a Gradient Boosting Regressor to predict weekly sales using store and department-level features.
5. Model Evaluation:
Assessed performance using RMSE, exported predictions to walmart_forecasts.csv, and visualized actual vs predicted sales.
6. Dashboard Development:
Imported final datasets into Power BI and built two dashboards:
7. Forecast Performance Dashboard
8. Store & Category Insights Dashboard
Implemented DAX measures such as Forecast Accuracy (%) and Total Predicted Sales.
9. Business Insight Generation:
Derived actionable insights on sales performance, holiday impact, and store type contribution.

🧩 Dashboards & DAX Measures
1. Forecast Performance Dashboard

KPIs:
Total Actual Sales: SUM(Weekly_Sales)
Total Predicted Sales: SUM(Predicted_Weekly_Sales)
Forecast Accuracy (%):
RMSE: Imported from Python model output.
Visuals: Weekly Sales Trend (Actual vs Predicted), Top 10 Stores by Sales, Sales by Store Type, and slicers for Year, Month, Holiday.

2. Store & Category Insights Dashboard
Visuals: Department-wise performance, Store Type comparison, Weekly Sales vs Temperature line chart, and Holiday filters.
Measures: Average Sales, Category Contribution (%), Store Count, and Holiday Impact.

🚀 Impact

1. Improved forecast accuracy, reducing overstocking and stockouts across multiple stores.
2. Enabled data-driven inventory planning, optimizing supply chain efficiency.
3. Provided real-time insights through interactive Power BI dashboards.
4. Enhanced decision-making for promotions, holidays, and seasonal demand.
5. Demonstrated the integration of Python ML models with Power BI analytics, bridging predictive and business intelligence workflows.

💡 Key Insights
| Area              | Observation                                       |
| ----------------- | ------------------------------------------------- |
| Forecast Accuracy | Maintained >90% accuracy across most stores.      |
| Seasonality       | High sales during holidays and promotions.        |
| Store Type        | Type A stores generated maximum sales.            |
| Drivers           | Temperature and lag features were key predictors. |
| Business Value    | Enabled better supply chain and demand planning.  |

🛠️ Tools & Technologies
| Category        | Tools Used                             |
| --------------- | -------------------------------------- |
| Programming     | Python (pandas, numpy, scikit-learn)   |
| Visualization   | Power BI                               |
| Query Language  | DAX (Power BI Measures)                |
| Modeling        | Gradient Boosting Regressor            |
| Data Processing | Label Encoding, Lag & Rolling Features |
| Evaluation      | RMSE, Forecast Accuracy %              |

🎯 Outcomes
| Aspect               | Description                                                  |
| -------------------- | ------------------------------------------------------------ |
| ML Pipeline          | Merged 4 datasets, built time-series model for weekly sales. |
| Power BI Integration | Linked Python outputs with Power BI KPIs & visuals.          |
| DAX Metrics          | Created Forecast Accuracy %, Total Sales, and RMSE cards.    |
| Forecast Results     | Achieved stable predictive performance across stores.        |
| Skillset             | Strengthened Python ML, DAX, and Power BI dashboard design.  |

