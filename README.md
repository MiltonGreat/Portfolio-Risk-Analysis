# Portfolio Risk Analysis

![screenshot-localhost_8888-2025 03 30-16_39_34](https://github.com/user-attachments/assets/004398d2-83cd-4835-8a24-5edf5711fc30)

### Project Overview

This project aims to perform Portfolio Risk Analysis using Value at Risk (VaR) and Expected Shortfall (CVaR) to assess the downside risk of stocks, with a focus on Apple Inc. (AAPL). By applying three different methods of calculating VaR (normal distribution, historical, and t-distribution), the project identifies the maximum potential loss within a specific confidence level and the average loss beyond that threshold.

The project also evaluates the Annualized Volatility of Apple Inc. stocks to understand its risk profile. These methods provide insights into potential extreme losses and are essential for managing investment portfolios effectively.

### Dataset

The analysis focuses on Apple Inc. (AAPL) stock data, specifically its Adjusted Close price, which is adjusted for splits and dividends. The dataset includes the following columns:

- Ticker: Stock symbol (e.g., AAPL)
- Date: Date of the stock price
- Open: Opening price for the day
- High: Highest price for the day
- Low: Lowest price for the day
- Close: Closing price for the day
- Adj Close: Adjusted closing price (used in the analysis)
- Volume: Number of shares traded

### Project Structure

1. Built portfolio_risk_analysis.py: Contains the core functions for calculating VaR, CVaR, and annualized volatility.
   
- calculate_var(): Computes VaR using three different methods (normal, historical, t-distribution).
- full_risk_analysis(): Computes a complete set of risk metrics including VaR, CVaR, and annualized volatility, and visualizes the risk distribution.

2. Visualization: The analysis includes histograms of daily returns, overlaid with the normal distribution fit and VaR thresholds for better understanding of the risk profile.

### Risk Metrics Interpretation

The following metrics are calculated and interpreted from the analysis:

- Normal VaR (95%): The potential maximum loss expected with a 95% confidence level, assuming a normal distribution of returns.

- Historical VaR (95%): The potential maximum loss expected with a 95% confidence level, based on actual historical returns.

- T-Dist VaR (95%): The potential maximum loss expected with a 95% confidence level, assuming a t-distribution of returns (better for handling extreme events).

- CVaR (95%): The average loss expected beyond the VaR threshold, representing the risk of extreme losses.

- Annualized Volatility: The volatility of the stock's daily returns, annualized to represent the total risk over a year.

### Conclusion

By using Value at Risk (VaR) and Expected Shortfall (CVaR), this project allows for a comprehensive understanding of the downside risk in Apple Inc.'s stock price. The analysis provides insights into potential extreme losses, helping investors and risk managers better assess the risk exposure of their portfolios.

### Source

![S&P 500 Stock Data From Listing Day to 2023 from Kaggle](https://www.kaggle.com/datasets/pavankrishnanarne/s-and-p-500-stock-data-from-listing-day-to-2023)
