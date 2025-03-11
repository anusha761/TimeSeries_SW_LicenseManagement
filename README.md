# License Usage Forecasting for Enterprise Software Management
> This project focuses on forecasting enterprise software license usage for Microsoft 365 by analyzing historical monthly data. The goal is to help organizations optimize software license procurement and renewal strategies by identifying seasonal trends in license demand. Various time series analysis techniques have been applied, and different models have been fitted to generate accurate forecasts.

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)



## General Information
- Project Overview: Forecasts Microsoft 365 Enterprise License usage using historical monthly data to assist organizations in managing software procurement, license renewals, and budget allocation.
- Data Analysis: Applies time series techniques including decomposition (additive/multiplicative), stationarity tests, and ACF/PACF plotting to understand the data’s underlying patterns. The analysis reveals a clear seasonal pattern in Microsoft 365 license usage, with spikes occurring at the end of fiscal quarters, during budget renewals. These fluctuations align with corporate IT procurement cycles and workforce expansion during key hiring seasons, where new employees require software licenses. Additionally, there is a consistent upward trend in license adoption, driven by the increasing shift toward cloud-based subscription models. As more departments migrate to cloud environments, the demand for enterprise licenses continues to grow steadily. Furthermore, the data shows a strong correlation between license acquisitions and promotional periods, as Microsoft strategically offers discounts and renewal incentives around fiscal deadlines. These promotions encourage bulk renewals and new purchases, reinforcing the observed seasonal spikes in usage.
- Forecasting Method: Utilizes the SARIMA model (Seasonal AutoRegressive Integrated Moving Average) to generate accurate license usage forecasts.
- Impact of Promotions and Renewals: Incorporates exogenous variables (enterprise promotions, bulk purchase discounts) into the analysis using the SARIMAX model, which helps capture the effect of renewal incentives and budget cycles. A rolling forecast approach was implemented to extend predictions into 2025, ensuring each step used the most recent predicted values and exogenous factors, mimicking real-world forecasting systems used in production.
- Objective: Aims to provide actionable insights for businesses, helping them optimize software license allocation and avoid unnecessary expenses during peak renewal periods.



## Conclusions
In conclusion, the time series analysis successfully provided accurate passenger traffic forecasts for the airline's specific route. The SARIMAX model, which included promotional events as an exogenous variable, significantly improved forecast accuracy, resulting in lower RMSE and MAPE values compared to the SARIMA model. These findings will help the airline optimize resource allocation during peak periods.




## Technologies Used
- pandas - version 2.2.2
- numpy - version 1.26.4
- matplotlib - version 3.7.1
- seaborn - version 0.13.2
- scikit-learn - version 1.5.2
- scipy - version 1.13.1
- statsmodel - 0.14.4
- scikit-learn - 1.6.1



  ## Contact
  Anusha Chaudhuri [anusha761]
