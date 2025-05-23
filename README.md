# Renewable Energy Forecasting in the National Electricity Market (NEM)
This repository contains the final research project for IFN695 – Integration Analysis and Impact Forecast. The goal is to analyze the growth of renewable energy in Australia’s National Electricity Market (NEM), evaluate forecasting techniques, and assess the impact of renewables on grid dynamics in high-adoption regions like Queensland.

# Project Objectives
1. Analyze the historical evolution of renewable energy penetration in the NEM (2023–2025).
2. Assess the impact of renewable sources on grid stability, ramp rates, and market dynamics.
3. Evaluate forecasting performance of models: ARIMA, XGBoost, and LSTM.
4. Compare Queensland with other high-renewable states (NSW, VIC).
5. Identify potential improvements for forecasting accuracy and grid resilience.
   
# Methodology Overview
- **Data Source**: Australian Energy Market Operator (AEMO) SCADA + NEM registration datasets.
- **Preprocessing**: Merging dispatch and registration data, filtering by DUID and region.
- **EDA**: Renewable share %, ramp rate, volatility, and regional generation mix.
- **Models Used**:
  - ARIMA (manual & auto-ARIMA)
  - XGBoost (lag-feature supervised learning)
  - LSTM (sequential time-series prediction using 7-day history)
- **Evaluation Metrics**:
  - RMSE, MAE, MAPE, R² Score
    
# Key Results
- **LSTM** achieved the best forecast performance with ~9.9% MAPE.
- **ARIMA** struggled with non-linearity, showing lower R² and higher error.
- **XGBoost** provided strong, interpretable results with minimal preprocessing.
- Queensland showed a steady renewable growth trend from ~18% in Jan 2023 to ~25% in Apr 2025.

