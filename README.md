# AAPL Stock Price Forecasting

## Installation

To use this code, you'll need to have the following Python packages installed:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `yfinance`
- `pmdarima`
- `tensorflow`

You can install these packages using pip:

```
pip install numpy pandas matplotlib scikit-learn yfinance pmdarima tensorflow
```

## Usage

The code is divided into several parts:

1. **Setup & Install**: This section imports the necessary libraries and ensures they are installed.
2. **Download Data**: This part downloads the AAPL stock data from Yahoo Finance.
3. **Feature Engineering**: This section creates some simple exogenous features for the SARIMAX model.
4. **Train/Test Split**: This part splits the data into training and testing sets.
5. **Metrics Helpers**: This section defines some helper functions for evaluating the model performance.
6. **ARIMA (auto)**: This part fits an ARIMA model using the `auto_arima` function from the `pmdarima` library.
7. **SARIMA (auto, weekly seasonality)**: This section fits a SARIMA model with weekly seasonality using the `auto_arima` function.
8. **SARIMAX (auto with exogenous features)**: This part fits a SARIMAX model with exogenous features using the `auto_arima` function.
9. **LSTM (windowed supervised learning)**: This section trains an LSTM model using TensorFlow.
10. **Results & Plots**: This part evaluates the model performance and generates a plot of the actual vs. predicted values.
11. **Save Outputs**: This section saves the model predictions and evaluation metrics to CSV files.
12. **Next-day Forecasts**: This part generates next-business-day forecasts for the models.

## API

The code does not provide a formal API, but it can be used as a starting point for your own stock price forecasting projects. You can modify the code to use different stock tickers, adjust the feature engineering, or experiment with different model architectures.

## Contributing

If you find any issues or have suggestions for improvements, feel free to open a GitHub issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Testing

The code includes some basic error handling and fallback mechanisms, but it does not have a comprehensive test suite. It is recommended to thoroughly test the code with different datasets and configurations before using it in a production environment.