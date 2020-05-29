# Production Optimization

One of the primary goals for companies across industries is to optimize their resources. Doing so leads to increased profit margins and a competitive advantage in the market. In the conxtext of manufacturing industries one way to do this is to optimize their production while avoididing 1) under-production which results in the loss of revenues 2) over-production which could result in storage costs and cash iliquidity. 

## Focusing on Demand Forecasting
An earnest attempt to optimize production in manufacturing requires a good understanding of both supply an demand factors for a particular industry. Because organizations usually have a greater authority over their supply factors, in this project we focused on forecasting demand. Having greater knowledge of the upcoming demand can help organizations optimize the use of their resources through the use of techniques like math optimization.


# Data
In this project we explore the use of multiple Time-Series models to forecast the demand for a steel manufacturing mill with sample data collected from 2016-2019.

## Data Table

| Name | Definition |
| ---- | ---------- |
|Calendar_day | Corresponding date in week, month or daily values|
|Shipment_tons|Target variable. The real demand, in tons|
|Inventory_tons|Inventory we have on hand, in tons|
|Sale_order_tons|Orders received that corresponded for that time(week/mo), in tons|
|Production_tons|Amount of production for that time, in tons|
|Carbon_bar_ship_canada|Aggregate shipment in tons for carbon bars in Canada|
|State_local_construction|Total construction in Billions of USD funded by states & local|
|Structural_ship_canada|Aggregate shipment for structural steel products in Canada, tons.|
|Carbon_bar_ship_usa|Aggregate amount of shipment for carbon bars in USA, in tons|
|Structural_ship_usa|Aggregate amount of shipment for structural steel products in USA, in tons|
|Global_steel_utilization|Global production level of steel|
|Ism_non_manufacturing|Index of expenditure in non-manufacturing sectors|
|Ism_manufacturing|Index of expenditure in the manufacturing sectors|
|Chicago_scrap$ST|Price per ton for scrap metal in the Chicago market|
|Federal_construction$B|Total construction in Billions of USD funded by the federal govt.|

# Time-Series Models:  

Univariate   
1) ARMA 
2) Facebook Prophet

Univariate/Multivariate  
1) LSTM

# Insights & Future Work

Using 12-week aggregate demand forecasts as inputs along with our LSTM model seems to provide the best Mean Absolute Error (MAE) scores for weekly predictions. Using this model along with a math optimization solution could be used to further optimize an organization's production of goods. 

While this model is able to do predict at an individual product level pretty well, this limits the amount of data points for analysis. Further exploration in the future will be needed to find a model that can generalize better across products and thus leverage more data available across different product types produced by the same organization. 
