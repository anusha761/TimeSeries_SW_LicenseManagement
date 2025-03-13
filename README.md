# Forecasting Enterprise Software License Usage and Expenses
> This repository contains two projects focused on forecasting MS365 enterprise software license usage and expenses using time series modeling. One project forecasts IT department software expenses due to the licenses, while the other project forecasts license usage demand. Both projects aim to optimize software procurement, budget planning, and cost efficiency by identifying trends in historical data.

## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)



## General Information

#### Project 1 - License Expenses Forecasting
- Overview: Forecasts IT department expenses related to software licenses to ensure cost-effective budgeting.
- Data Analysis: Applies time series techniques including decomposition (additive/multiplicative), stationarity tests, and ACF/PACF plotting to understand the data’s underlying patterns.The historical expense data exhibits an upward trend, reflecting the growing cost of software licenses over time. This steady increase suggests an expansion in enterprise software usage, possibly driven by organizational growth, new tool adoption, or changing licensing models. A seasonal pattern is also evident, with recurring peaks and dips at regular intervals. This cyclic behavior indicates that license expenses fluctuate in alignment with predefined business cycles, such as annual budget approvals, project renewals, or workforce expansions. The time series decomposition further confirms this, isolating the trend and seasonal variations from residual noise. Additionally, short-term fluctuations in the data highlight unexpected variations, possibly due to occasional bulk purchases, internal policy shifts, or vendor-driven pricing adjustments. These irregular movements emphasize the importance of forecasting, enabling businesses to anticipate and manage future expenses more effectively.
- Forecasting Method: Utilizes LSTM (Long Short Term Memory) type of Recurrent Neural Network to generate license expenses forecasts.
- Objective: Aims to ensure cost-effective budgeting
  
#### Project 2 - License Usage Forecasting
- Overview: Forecasts license usage to assist organization in managing software procurement, license renewals, and budget allocation.
- Data Analysis: Applies time series techniques including decomposition (additive/multiplicative), stationarity tests, and ACF/PACF plotting to understand the data’s underlying patterns. The analysis reveals a clear seasonal pattern in Microsoft 365 license usage, with spikes occurring at the end of fiscal quarters, during budget renewals. These fluctuations align with corporate IT procurement cycles and workforce expansion during key hiring seasons, where new employees require software licenses. Additionally, there is a consistent upward trend in license adoption, driven by the increasing shift toward cloud-based subscription models. As more departments migrate to cloud environments, the demand for enterprise licenses continues to grow steadily. Furthermore, license acquisitions are influenced by promotional periods, as vendors strategically offers discounts and renewal incentives around fiscal deadlines. These promotions encourage bulk renewals and new purchases, reinforcing the observed seasonal spikes in usage.
- Forecasting Method: Utilizes the SARIMA model (Seasonal AutoRegressive Integrated Moving Average) to generate license usage forecasts.
- Impact of Promotions and Renewals: Incorporates exogenous variables (enterprise promotions, bulk purchase discounts) into the analysis using the SARIMAX model, which helps capture the effect of renewal incentives and budget cycles. A rolling forecast approach was implemented to extend predictions into 2025, ensuring each step used the most recent predicted values and exogenous factors, mimicking real-world forecasting systems used in production.
- Objective: Aims to provide actionable insights for businesses, helping them optimize software license allocation and avoid unnecessary expenses during peak renewal periods.



## Conclusions
In conclusion, the time series analysis successfully provided decent forecasts for the future license expenses to bear and the demands. The LSTM model with dropout reduced the overfit and forecasted future expenses to bear. The SARIMAX model, which included promotional events as an exogenous variable, significantly improved forecast accuracy, resulting in lower RMSE and MAPE values compared to the SARIMA model. These findings will help the organization plan budget effectively and optimize license allocation. 




## Technologies Used
- pandas - version 2.2.2
- numpy - version 1.26.4
- matplotlib - version 3.7.1
- seaborn - version 0.13.2
- scikit-learn - version 1.5.2
- scipy - version 1.13.1
- statsmodel - 0.14.4
- scikit-learn - 1.6.1
- tensorflow - 2.18.0
- keras - 3.8.0


  ## Contact
  Anusha Chaudhuri [anusha761]
