# Climate-change
Building a predictive ML models for climate change
The project focuses on analyzing global climate data (2000–2023) to build machine learning models capable of predicting future temperature rise, sea-level changes, and extreme weather events.
Here is a breakdown of the methodology, the challenges, and what the data revealed. 
The Approach: Time-Series Modeling
Using a dataset covering 24 years of global climate aggregates, I engineered features including lag variables (1 & 2 years), rolling means, and interaction terms (like CO2 per Renewable Energy %).
I tested four models: Linear Regression, Ridge, Random Forest, and Gradient Boosting. To avoid data leakage, I used Time Series Split cross-validation—a critical step when predicting the future.
Feature Importance: The Drivers of Change
The Random Forest and Gradient Boosting models revealed the most impactful predictors:
🔥 Temperature: The interaction between Temperature and CO2 (Temp_CO2_index) was the #1 driver (32% importance).
🌊 Sea Level: Forest Area and Renewable Energy adoption (lagged) were surprisingly strong predictors.
⛈️ Extreme Weather: Past temperature (lagged) and CO2 indices drove event frequency.
4️⃣ The 10-Year Forecast (2024–2033)
Using a recursive one-step-ahead forecasting method, the models projected climate scenarios into the next decade:
Temperature: Expected to stabilize around 20.3°C – 20.5°C (down from the 2023 peak of 21.1°C, though historical volatility remains high).
Sea Level: Projected to hold steady around 3.02 mm.
Extreme Weather: Forecasted to average 7.3 events per year, showing slight volatility.
