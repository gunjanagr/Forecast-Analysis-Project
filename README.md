
# Forecast Analysis Project

## Overview
A time series forecasting solution implementing SARIMA models to analyze and predict future trends in temporal data. This project provides:
- Automated data preprocessing
- Model training and evaluation
- Interactive forecasting interface
- Performance visualization

## Features
- **Data Visualization**: Interactive time series decomposition and trend analysis
- **SARIMA Modeling**: Automated parameter selection (p,d,q)(P,D,Q)s
- **Performance Metrics**: MAE, RMSE, and MAPE calculations
- **Historical Forecasts**: Backtesting capabilities with visual comparison

## Installation
1. Clone repository:git clone https://github.com/gunjanagr/Forecast-Analysis-Project.git
cd Forecast-Analysis-Project
2. Install dependencies:pip install -r requirements.txt
   
## Usage
1. Prepare your time series data in CSV format with:
   - A single column of numerical values
   - DateTime index (optional)


## Key Functionality
### Data Preprocessing
- Missing value imputation
- Stationarity checks (ADF test)
- Seasonal decomposition

### Model Training
model = SARIMAX(train_data, order=(1,1,1), seasonal_order=(1,1,1,12))
results = model.fit()

### Forecasting
- Dynamic predictions with confidence intervals
- Multi-step ahead forecasting

## Results

| Metric | Value |
|--------|-------|
| MAE    | 2.34  |
| RMSE   | 3.15  |
| MAPE   | 4.5%  |

## Streamlit Interface
Interactive features include:
- Date range selection
- Model parameter adjustments
- Forecast horizon control
- Interactive results visualization

## Synopsis 
1. Loaded the dataset and parsed the 'datetime' column.
2. Handled missing values in the 'load' column using mean imputation.
3. Used the Holt-Winters model for forecasting with seasonality and trend components.
4. Forecasted the load values for December 14, 2020, at 15-minute intervals.
5. Saved the results as a CSV file: {forecast_csv_path}.
   ## Conclusion
The Forecast Analysis Project demonstrates the application of SARIMA models for time series forecasting, providing insights into data trends and future predictions. This project serves as a valuable tool for anyone looking to understand and implement forecasting techniques in their own datasets.

## Contact
For any inquiries or suggestions, feel free to reach out:
- Email: [gunjagr02@gmail.com]
- GitHub: [https://github.com/gunjanagr]

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.






