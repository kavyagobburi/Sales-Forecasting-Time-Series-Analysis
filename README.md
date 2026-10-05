# Sales-Forecasting-Time-Series-Analysis
Project Overview

A self-initiated Data Analyst portfolio project focused on analyzing historical sales trends and building a short-term sales forecast.

The project uses two years of daily sales data to demonstrate data cleaning, time-series analysis, visualization, and forecasting using Python and Prophet.

Business Problem

A business wants to understand historical sales performance and use past sales patterns to estimate future sales for planning and decision-making.

Objectives
Clean and validate daily sales data.
Analyze monthly sales performance and growth.
Identify historical high and low sales periods.
Visualize sales trends and forecasting patterns.
Build a 6-month sales forecast.
Document assumptions and forecasting limitations.
Tools & Technologies
Python
Pandas
Matplotlib
Prophet
Excel
Jupyter Notebook
Dataset

The dataset contains 731 daily sales records covering January 2024 through December 2025.

Columns:

Date
Sales

The dataset was created for portfolio analysis and represents a synthetic sales scenario.

Data Cleaning

The raw dataset contained intentionally introduced data-quality issues:

Missing Sales value
Negative Sales value
Duplicate Date

Cleaning steps included:

Loaded the Excel dataset using Pandas.
Interpolated the missing Sales value.
Converted Date to datetime format.
Removed duplicate dates.
Replaced the negative Sales value using the median of valid sales values.
Sorted the data by Date.
Performed final data-quality checks.
Analysis
Monthly Sales Analysis

Daily sales were aggregated into monthly totals using Pandas.

The analysis included:

Monthly sales totals
Month-over-month sales growth
Highest historical sales month
Lowest historical sales month
Sales trend visualization
Forecasting

Prophet was used to forecast the next 6 months of sales.

The forecasting workflow included:

Prepared monthly sales data in Prophet format using ds and y.
Configured yearly seasonality.
Trained the Prophet model.
Generated a 6-month future date range.
Generated forecast values with lower and upper estimates.
Visualized the forecast and model components.
Forecast Output

The forecast results contain:

Forecast month
Forecast sales
Lower estimate
Upper estimate

The forecast is intended as an analytical estimate for planning rather than a guaranteed future result.

Project Structure
Sales-Forecasting-Time-Series-Analysis/
│
├── README.md
│
├── python/
│   └── Project3_Sales_Forecasting.ipynb
│
├── data/
│   └── Project3_Sales_Forecasting_Raw_Data.xlsx
│
└── outputs/
    ├── Project3_Sales_Forecast_Results.xlsx
    ├── Project3_Monthly_Sales_Analysis.xlsx
    └── Project3_Final_Forecast_Summary.xlsx
Key Skills Demonstrated
Data cleaning with Pandas
Data-quality validation
Time-series aggregation
Month-over-month growth analysis
Data visualization with Matplotlib
Forecasting with Prophet
Forecast interpretation
Business-oriented analytical reporting
Documenting assumptions and limitations
Business Use

Sales forecasts can support:

Sales planning
Inventory planning
Resource allocation
Budgeting
Promotional planning
Monitoring expected future demand
Limitation

The project uses two years of historical data, with 24 monthly observations used for the monthly forecasting model. Because the historical period is limited, the forecast should be interpreted as an estimate and not as a guaranteed prediction.

The dataset is synthetic and was created for portfolio demonstration purposes.

Project Type

Self-initiated portfolio project

This project does not represent work performed for a real client or employer.
