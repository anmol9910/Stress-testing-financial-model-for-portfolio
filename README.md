# S&P 500 Portfolio Stress Testing & Sectoral Analysis

## Project Overview

This project provides a comprehensive analysis of S&P 500 historical stock data over a five-year period. The primary goal is to assess the resilience of a financial portfolio against severe market shocks through simulation and to conduct a comparative analysis of performance across different industry sectors. The framework is built in Python using core data science libraries for data manipulation, analysis, and visualization.

## Key Features & Analysis Performed

-   **Data Aggregation:** Processed and combined historical data from over 500 individual company CSV files into a single, unified Pandas DataFrame for analysis.
-   **Scenario-Based Stress Testing:**
    -   **Financial Crisis Simulation:** Modeled the impact of a severe market crash (e.g., a 30% drop in stock prices) on the portfolio's cumulative returns.
    -   **Interest Rate Hike Simulation:** Modeled the impact of a smaller, systemic shock (e.g., a 10% drop) representing an interest rate hike scenario.
-   **Performance Visualization:** Plotted and compared the cumulative returns of the portfolio under normal conditions versus stressed scenarios to visualize impact and recovery paths.
-   **In-Depth Sectoral Analysis:**
    -   Grouped all stocks by their respective industries (e.g., Information Technology, Health Care, Energy).
    -   Calculated and visualized comparative metrics, including **average stock price, trading volume, daily returns, and volatility (risk)** for each sector.
-   **Correlation Analysis:** Generated a correlation heatmap to understand the relationships between different sectors, providing key insights for portfolio diversification.

## Technology Stack

-   **Language:** Python
-   **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
-   **Environment:** Jupyter Notebook / Kaggle

## Methodology

The project follows a three-step methodology:
1.  **Data Preprocessing:** Loading, cleaning, and aggregating the raw stock data.
2.  **Simulation:** Applying rule-based scenarios to the dataset to create "stressed" portfolio values.
3.  **Analysis & Visualization:** Grouping the data by industry and using statistical measures and plots to extract meaningful insights.

## Future Work & Potential Improvements

While the current analysis provides a solid foundation, the following advanced techniques could be implemented to further enhance this project:
-   **Implement Statistical Risk Models:** Calculate and analyze **Value at Risk (VaR)** and **Conditional Value at Risk (CVaR)** to quantify potential losses with specific confidence levels.
-   **Integrate Factor Models:** Use multi-factor models like the **Fama-French Three-Factor Model** to conduct a more sophisticated stress test and explain the drivers of portfolio returns.
-   **Liquidity Risk Assessment:** Develop a model to assess liquidity risk by analyzing trading volumes and simulating scenarios where assets cannot be easily sold at their market price.
-   **Build an Interactive Dashboard:** Create a web-based dashboard using Streamlit or Plotly Dash to allow users to interact with the simulations and analysis dynamically.

---

## About the Dataset (Source: Kaggle)

-   **Content:** The dataset provides historical stock prices (Open, High, Low, Close, Volume) for S&P 500 companies, updated as of February 2018. The data is available as a single merged file (`all_stocks_5yr.csv`) and as individual files for each stock.
-   **Acknowledgements:** The data was sourced from The Investor's Exchange (IEX) API.
