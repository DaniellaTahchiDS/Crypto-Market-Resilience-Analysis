# Crypto Market Resilience Analysis

A comprehensive comparative analysis of Bitcoin and Ethereum, examining their inflation hedging potential, macroeconomic correlation, and overall market dynamics. This project investigates whether these major cryptocurrencies can truly serve as inflation hedges or remain primarily speculative growth assets under changing economic conditions.

## 🎯 Project Overview

This analysis aims to understand the resilience and behavior of Bitcoin (BTC) and Ethereum (ETH) in various economic environments by examining:

- **Inflation Hedging Potential**: Can these cryptocurrencies protect against inflation?
- **Macroeconomic Correlations**: How do they respond to traditional market indicators?
- **Market Dynamics**: What drives price movements and volatility?
- **Comparative Performance**: How do BTC and ETH differ in their market behavior?

## 📊 Key Research Questions

1. Do Bitcoin and Ethereum exhibit properties of traditional inflation hedges (like gold)?
2. How correlated are these cryptocurrencies with:
   - Traditional equity markets (S&P 500, NASDAQ)
   - Treasury yields and interest rates
   - Inflation metrics (CPI, PCE)
   - Dollar strength (DXY)
3. What are the key drivers of cryptocurrency price movements?
4. How do market conditions (bull vs. bear markets) affect their hedging properties?

## 🔧 Methodology

### Data Collection
- **Cryptocurrency Data**: Historical price, volume, and market capitalization data
- **Macroeconomic Data**: Inflation rates, interest rates, GDP growth, unemployment
- **Market Indices**: S&P 500, NASDAQ, gold prices, DXY (Dollar Index)
- **Time Period**: [Specify your data range]

### Analysis Techniques
- **Time Series Analysis**: Examining price trends, volatility, and returns
- **Correlation Analysis**: Measuring relationships with macroeconomic variables
- **Regression Models**: Identifying key drivers of cryptocurrency prices
- **Rolling Correlations**: Analyzing time-varying relationships
- **Volatility Clustering**: Using GARCH/EGARCH models
- **Event Studies**: Impact of major economic events on crypto prices

## 📁 Repository Structure

```
Crypto-Market-Resilience-Analysis/
├── Data/
│   ├── BNB.csv                          # Binance Coin historical data
│   ├── BTC.csv                          # Bitcoin historical data
│   ├── ETH.csv                          # Ethereum historical data
│   ├── ExchangeRate.csv                 # Currency exchange rates
│   ├── GoogleTrends.csv                 # Google search trends data
│   ├── InflationRate.csv                # Historical inflation metrics
│   ├── UnemploymentRate.csv             # Unemployment statistics
│   └── majorevent.csv                   # Major economic/market events
├── notebook/
│   ├── BTCAnalysis.ipynb                # Bitcoin-focused analysis
│   ├── CryptoForecasting.ipynb          # Predictive modeling and forecasting
│   ├── CryptoVisualize.ipynb            # Data visualization notebook
│   ├── ETHAnalysis.ipynb                # Ethereum-focused analysis
│   ├── ETHvsBTC.ipynb                   # Comparative analysis of ETH and BTC
│   └── GoogleTrendsCryptoAnalysis.ipynb # Search trends correlation analysis
├── BTC vs ETH_Crypto Market Resilience Analysis.pdf  # Final research report
└── README.md                            # This file
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- pip or conda package manager

### Installation

1. Clone the repository:
```bash
git clone https://github.com/DaniellaTahchiDS/Crypto-Market-Resilience-Analysis.git
cd Crypto-Market-Resilience-Analysis
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

### Required Libraries
```
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
plotly>=5.11.0
scikit-learn>=1.1.0
statsmodels>=0.13.0
yfinance>=0.2.0
requests>=2.28.0
jupyter>=1.0.0
```

## 📈 Key Findings

### Bitcoin Analysis
- [Summary of Bitcoin's correlation with inflation]
- [Bitcoin's response to macroeconomic events]
- [Key drivers of Bitcoin price movements]

### Ethereum Analysis
- [Summary of Ethereum's correlation with inflation]
- [Ethereum's response to macroeconomic events]
- [Comparison with Bitcoin behavior]

### Comparative Insights
- [Key differences between BTC and ETH]
- [Which performs better as an inflation hedge?]
- [Market condition dependencies]

## 📊 Visualizations

The analysis includes comprehensive visualizations across multiple notebooks:

**CryptoVisualize.ipynb** contains:
- Price and volume trends over time
- Correlation heatmaps with macroeconomic variables
- Rolling correlation charts
- Volatility analysis and GARCH model outputs
- Return distributions and risk metrics

**Individual Analysis Notebooks** provide:
- Asset-specific technical indicators
- Moving averages and trend analysis
- Event impact studies with timeline markers
- Comparative performance charts

**Google Trends Analysis** shows:
- Search interest vs price correlation
- Sentiment indicators
- Regional interest patterns

## 🔍 Usage

### Exploring the Analysis

The analysis is organized into specialized Jupyter notebooks, each focusing on different aspects:

1. **Bitcoin Analysis** (`BTCAnalysis.ipynb`)
   - Comprehensive analysis of Bitcoin price movements
   - Correlation with macroeconomic indicators
   - Volatility and risk metrics

2. **Ethereum Analysis** (`ETHAnalysis.ipynb`)
   - In-depth Ethereum market analysis
   - Comparison of ETH characteristics vs traditional assets
   - Network effects and adoption metrics

3. **Comparative Analysis** (`ETHvsBTC.ipynb`)
   - Direct comparison between Bitcoin and Ethereum
   - Relative performance during different market conditions
   - Correlation analysis between the two cryptocurrencies

4. **Forecasting Models** (`CryptoForecasting.ipynb`)
   - Time series forecasting techniques
   - Predictive models for price movements
   - Model evaluation and validation

5. **Visualization Dashboard** (`CryptoVisualize.ipynb`)
   - Interactive visualizations of key findings
   - Trend analysis and pattern recognition
   - Comparative charts and heatmaps

6. **Google Trends Analysis** (`GoogleTrendsCryptoAnalysis.ipynb`)
   - Correlation between search interest and price movements
   - Public sentiment analysis
   - Leading indicators from search data

### Running the Notebooks

```bash
# Navigate to the notebook directory
cd notebook

# Launch Jupyter
jupyter notebook

# Open any notebook and run cells sequentially
```

### Example Code

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

# Load cryptocurrency data
btc_data = pd.read_csv('Data/BTC.csv')
eth_data = pd.read_csv('Data/ETH.csv')

# Load macroeconomic indicators
inflation = pd.read_csv('Data/InflationRate.csv')
unemployment = pd.read_csv('Data/UnemploymentRate.csv')

# Calculate correlation
correlation = btc_data['price'].corr(inflation['rate'])
print(f"BTC-Inflation Correlation: {correlation:.4f}")

# Visualize trends
plt.figure(figsize=(12, 6))
plt.plot(btc_data['date'], btc_data['price'], label='Bitcoin Price')
plt.plot(eth_data['date'], eth_data['price'], label='Ethereum Price')
plt.legend()
plt.show()
```

## 📚 Data Sources

The analysis utilizes multiple data sources to provide comprehensive coverage:

- **Cryptocurrency Price Data**: 
  - Bitcoin (BTC), Ethereum (ETH), and Binance Coin (BNB)
  - Historical price, volume, and market cap data
  
- **Macroeconomic Indicators**:
  - Inflation Rate: CPI and other inflation metrics
  - Unemployment Rate: Labor market statistics
  - Exchange Rates: Currency valuation data
  
- **Market Sentiment**:
  - Google Trends: Search interest and public sentiment
  - Major Events: Economic and market-moving events timeline
  
- **Additional Sources**:
  - CoinGecko/CoinMarketCap: Cryptocurrency market data
  - Federal Reserve Economic Data (FRED): Economic indicators
  - Bureau of Labor Statistics (BLS): Employment data

## 🔬 Methodology Details

### Statistical Techniques
1. **Pearson/Spearman Correlation**: Measuring linear and monotonic relationships
2. **Granger Causality Tests**: Testing predictive relationships
3. **VAR Models**: Vector autoregression for multivariate time series
4. **GARCH Models**: Modeling volatility clustering
5. **Cointegration Analysis**: Testing long-term equilibrium relationships

### Challenges & Limitations
- **Data Availability**: Cryptocurrency markets are relatively young
- **Market Maturity**: Rapidly evolving market structure
- **External Factors**: Regulatory changes, technological developments
- **Sample Size**: Limited data for certain economic regimes

## 📝 Results & Conclusions

The complete analysis and findings are documented in the research report: **[BTC vs ETH_Crypto Market Resilience Analysis.pdf](BTC%20vs%20ETH_Crypto%20Market%20Resilience%20Analysis.pdf)**

### Key Analysis Areas

This project explores:

1. **Inflation Hedging Effectiveness**
   - Analyzing whether BTC and ETH can protect against inflation
   - Comparing their performance to traditional hedges (gold, commodities)
   - Time-varying correlation analysis with CPI data

2. **Macroeconomic Sensitivity**
   - Response to interest rate changes
   - Correlation with unemployment and economic growth
   - Impact of major economic events

3. **Market Dynamics**
   - Volatility patterns and clustering
   - Price momentum and trends
   - Volume analysis and liquidity considerations

4. **Comparative Performance**
   - Bitcoin vs Ethereum characteristics
   - Risk-adjusted returns
   - Market maturity and adoption metrics

5. **Sentiment Analysis**
   - Google Trends correlation with price movements
   - Public interest as a leading/lagging indicator
   - Media attention impact

### Main Takeaways

For detailed findings, insights, and conclusions, please refer to the [full research report](BTC%20vs%20ETH_Crypto%20Market%20Resilience%20Analysis.pdf) included in this repository.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

Daniella Tahchi - [@DaniellaTahchiDS](https://github.com/DaniellaTahchiDS)

Project Link: [https://github.com/DaniellaTahchiDS/Crypto-Market-Resilience-Analysis](https://github.com/DaniellaTahchiDS/Crypto-Market-Resilience-Analysis)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [CoinGecko](https://www.coingecko.com/) for cryptocurrency data
- [Federal Reserve Economic Data (FRED)](https://fred.stlouisfed.org/) for macroeconomic data
- [Yahoo Finance](https://finance.yahoo.com/) for traditional market data
- Academic research on cryptocurrency market dynamics

## 📚 References

1. Baur, D. G., & Lucey, B. M. (2010). Is gold a hedge or a safe haven? An analysis of stocks, bonds and gold. *Financial Review*.
2. Klein, T., Thu, H. P., & Walther, T. (2018). Bitcoin is not the New Gold–A comparison of volatility, correlation, and portfolio performance. *International Review of Financial Analysis*.
3. Corbet, S., Meegan, A., Larkin, C., Lucey, B., & Yarovaya, L. (2018). Exploring the dynamic relationships between cryptocurrencies and other financial assets. *Economics Letters*.
4. [Add your own references]

---

**Note**: This is an academic research project. The findings should not be considered as financial advice. Cryptocurrency investments carry significant risk.
