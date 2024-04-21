# Sales Forecasting Project for Siemens

## Overview
This repository documents a comprehensive sales forecasting project conducted for Siemens, focusing on predicting monthly sales for selected product groups within the Smart Infrastructure Division. The project employed rigorous analysis and modeling efforts, following the CRISP-DM framework.

## Project Phases
### Data Understanding
- Descriptive statistics and data visualization techniques were utilized to understand the characteristics of market data and sales data.
- Insights were derived regarding sales patterns, seasonality, and correlations among variables.

![output](https://github.com/DiogoPimenta26/Siemens-Advanta-Sales-Forecast/assets/148448280/5852a109-dba3-40ec-ac00-cf76956aaeee)


![2](https://github.com/DiogoPimenta26/Siemens-Advanta-Sales-Forecast/assets/148448280/438abadb-fabd-4788-ab9e-df0d62956646)

### Data Preparation
- Extensive feature engineering integrated macroeconomic indicators, seasonal factors, and lag features into the dataset.
- Missing values were addressed through predictive imputation.
- Feature selection techniques were employed to identify the most relevant variables for modeling, eliminating redundancies.

### Modeling and Evaluation
- Various machine learning models, including KNN, Linear Regression, Random Forest, XGBoost, Ensemble, and SARIMAX, were applied to forecast sales for different product groups.
- Models were evaluated based on Root Mean Square Error (RMSE) values, with lower RMSE indicating better predictive performance.


| GCK | Features Selected                                                                                                   |
|-----|----------------------------------------------------------------------------------------------------------------------|
| 1   | '12 Month EMA','production index: Germany: Electrical equipment_lag_3','MACD Histogram','production index: United Kingdom: Electrical equipment_lag_1'                                         |
| 3   | 'Signal Line', 'MACD', 'production index: World: Electrical equipment','Italy:Production Index Machinery & Electricals_lag_3','China:Production Index Machinery & Electricals_lag_3' |
| 4   | '12 Month EMA', 'MACD Histogram', '26 Month EMA','production index: Switzerland: Machinery and equipment n.e.c._lag_6'                                                           |
| 5   | 'US:Shipments Index Machinery & Electricals_lag_3','MACD Histogram','France:Production Index Machinery & Electricals_lag_1','production index: Japan: Electrical equipment_lag_1' |
| 6   | 'Italy:Shipments Index Machinery & Electricals_lag_1','Switzerland:Production Index Machinery & Electricals_lag_6','MACD','MACD Histogram', 'US:Production Index Machinery & Electricals','France:Production Index Machinery & Electricals_lag_5','UK:Shipments Index Machinery & Electricals' |
| 8   | '12 Month EMA','MACD Histogram','production index: United Kingdom: Electrical equipment_lag_6', 'World: Price of Natural gas index','Sales_EUR_Lag_3'                                    |
| 9   | '12 Month EMA','Sales_EUR_Lag_6','Sales_EUR_Lag_2', 'MACD','MACD Histogram','production index: Japan:Electrical equipment','Sales_EUR_Lag_8'                                             |
| 11  | 'MACD Histogram', 'MACD'                                                                                             |
| 12  | 'MACD Histogram','12 Month EMA','MACD','Sales_EUR_Lag_6', 'Italy:Shipments Index Machinery & Electricals','UK:Production Index Machinery & Electricals','World: Price of Energy' |
| 13  | 'MACD Histogram','production index: Switzerland: Electrical equipment','Sales_EUR_Lag_3','production index: Switzerland: Machinery and equipment n.e.c.','Sales_EUR_Lag_7','China:Production Index Machinery & Electricals_lag_2','MACD','production index: Germany: Electrical equipment_lag_5','production index: World: Electrical equipment_lag_4','Signal Line' |
| 14  | 'MACD Histogram','MACD','Europe:Production Index Machinery & Electricals_lag_4','UK:Production Index Machinery & Electricals_lag_4','production index: Japan: Electrical equipment', 'production index: Germany: Electrical equipment_lag_4' |
| 16  | 'Producer Prices: Germany: Electrical equipment_lag_6','MACD', '12 Month EMA'                                         |
| 20  | 'MACD Histogram','Producer Prices: Germany: Electrical equipment_lag_4','World: Price of Energy_lag_6','12 Month EMA'                                                               |
| 36  | 'MACD Histogram','Europe:Production Index Machinery & Electricals_lag_2','Producer Prices: China: Electrical equipment_lag_5','US:Shipments Index Machinery & Electricals_lag_5', 'Sales_EUR_Lag_2','Italy:Shipments Index Machinery & Electricals_lag_3' |


## Results
- Promising outcomes were observed, with different models performing optimally for different product groups.
- For example, Linear Regression yielded the lowest RMSE for GCK 4 and GCK 5, while Random Forest performed well for GCK 6 and GCK 8.

| Model             | RMSE            | Mapped_GCK |
|-------------------|-----------------|------------|
| KNN               | 2574299,846     | 1          |
| Linear Regression | 1071342,997     | 3          |
| Linear Regression | 111325,6246     | 4          |
| Linear Regression | 2718332,028     | 5          |
| Random Forest     | 113122,5668     | 6          |
| Random Forest     | 303534,0265     | 8          |
| Linear Regression | 7575,82085      | 9          |
| Random Forest     | 1094146,122     | 11         |
| Linear Regression | 82851,78045     | 12         |
| Linear Regression | 11282,3649      | 13         |
| Linear Regression | 14084,54736     | 14         |
| XGBoost           | 65993,26114     | 16         |
| Ensemble          | 1104,632418     | 20         |
| Random Forest     | 10337,89908     | 36         |


## Deployment and Maintenance
- Plans for deployment and maintenance were outlined to ensure the continued relevance and effectiveness of the sales forecasting model.
- Strategies for model improvement were discussed, including implementing correlation of product sales, utilizing grid search for model optimization, and exploring alternative feature selection metrics.

## Repository Contents
- Data Understanding: Descriptive statistics and data visualization notebooks.
- Data Preparation: Feature engineering and missing value imputation scripts.
- Modeling and Evaluation: Machine learning model implementation and evaluation notebooks.
- Deployment and Maintenance: Documentation on deployment strategies and model maintenance plans.

## Future Work
- Continual model improvement strategies, such as implementing correlation of product sales and exploring alternative feature selection metrics.
- Updating the model with new data to ensure its relevance and accuracy over time.


