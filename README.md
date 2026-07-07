# Demand Forecasting for Retail

## Project Overview
This project focuses on forecasting product demand for a retail store to optimize inventory levels and prevent stockouts. Using historical sales data from Walmart, the pipeline incorporates calendar holidays and promotional markdowns to build an accurate predictive timeline.

## Dataset
The dataset utilized is the **Walmart Cleaned Data**, which includes:
* **Target:** `Weekly_Sales` (Segmented by Store and Department)
* **Features:** `IsHoliday`, `MarkDown1-5`, `Temperature`, `Fuel_Price`, `CPI`, and `Unemployment`

## Methodology & Models
* **Data Preprocessing:** Handled date formats, isolated a single high-volume store/department time series, and checked data features.
* **Modeling:** Implemented **Facebook Prophet**, a robust additive regression model designed for time-series data with strong seasonal components and tracking of exogenous promotional events.
* **Evaluation:** Performance was assessed using **RMSE** (Root Mean Squared Error) and **MAPE** (Mean Absolute Percentage Error).

## Results & Insights
* **Model Accuracy:** achieved via Prophet forecasting.
* **Business Application:** Translated forecast results into operational inventory logic by calculating the **Safety Stock** buffer and establishing a concrete **Reorder Point (ROP)**.
