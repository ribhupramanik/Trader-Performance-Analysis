# 📊 Relationship Between Trader Performance and Market Sentiment

## Project Overview

This project explores the relationship between **Bitcoin Market Sentiment** and **trader performance** using historical trading data from Hyperliquid.

The analysis combines a daily Bitcoin Fear & Greed Index with historical trading records to examine how different market sentiment conditions relate to trader profitability, trading behaviour, and market activity.

---

## Objective

The objective of this project is to:

- Merge Bitcoin market sentiment data with historical trading data.
- Analyze trader performance across different market sentiment categories.
- Explore how profitability, trade size, fees, and trading activity change under different market conditions.
- Present insights using data visualization and exploratory data analysis (EDA).

---

## Dataset

The project uses two datasets:

### 1. Bitcoin Market Sentiment Dataset

Contains daily market sentiment classifications:

- Date
- Classification
  - Extreme Fear
  - Fear
  - Neutral
  - Greed
  - Extreme Greed

### 2. Historical Trader Dataset (Hyperliquid)

Contains historical trading information including:

- Account
- Coin
- Side (BUY / SELL)
- Size USD
- Closed PnL
- Fee
- Execution Price
- Timestamp
- Other trading-related attributes

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Preparation

The following preprocessing steps were performed:

- Loaded both datasets.
- Converted timestamps into a common date format.
- Cleaned and standardized column names.
- Merged the datasets using the trading date.
- Created a **Win** indicator based on whether the Closed PnL was positive.

---

## Exploratory Data Analysis

The notebook includes the following analyses:

- Market sentiment distribution
- Average Closed PnL by market sentiment
- Median Closed PnL by market sentiment
- Total Closed PnL by market sentiment
- Average trade size by market sentiment
- Average trading fees by market sentiment
- Win rate across market sentiment categories
- Coin-wise average profitability
- Top performing trading accounts
- Daily profit trend
- BUY vs SELL distribution across market sentiment
- Profit distribution using boxplots
- Correlation analysis between Closed PnL, Fee, and Trade Size

---

## Key Findings

The analysis highlights several observable patterns:

- Trading activity is concentrated in the Fear and Greed market conditions.
- Average profit per trade differs across market sentiment categories.
- Fear markets generate the highest cumulative profit because of higher trading activity.
- Median Closed PnL remains close to zero across all sentiment classes, indicating that overall profitability is influenced by a relatively small number of highly profitable trades.
- Average trade size and average trading fees vary across different market conditions.
- Win rates differ across sentiment categories.
- Coin performance is not uniform across different market sentiment conditions.
- Top-performing accounts generate profits under multiple market conditions.
- Daily trader profitability is highly volatile.
- Trade size shows a strong positive relationship with trading fees, while its relationship with profitability is comparatively weak.

---

## Repository Structure

```
.
├── Relationship_between_trader_performance_and_market_sentiment.ipynb
├── historical_data.csv
├── fear_greed_index.csv
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/ribhupramanik/trader-performance-market-sentiment-analysis.git
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
Relationship_between_trader_performance_and_market_sentiment.ipynb
```

and run all cells.

---

## Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
```

---

## Conclusion

This project demonstrates how exploratory data analysis can be used to investigate the relationship between market sentiment and trading performance.

By combining market sentiment data with historical trading records, the notebook provides visual insights into trader profitability, trading activity, position behaviour, and transaction characteristics across different market conditions.

The analysis serves as a foundation for understanding how sentiment can be incorporated into trading analysis and highlights several patterns that may be useful for further quantitative research.

---

## Author

**Ribhu Pramanik**

GitHub: https://github.com/ribhupramanik