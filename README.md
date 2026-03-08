## Project Overview

This project explores how market sentiment (Fear vs Greed) affects trader behavior and profitability on the Hyperliquid platform. The goal of this analysis is to understand whether traders behave differently during different market sentiment conditions and whether this impacts their performance.

The analysis combines two datasets:
1. Bitcoin Fear & Greed Index (market sentiment)
2. Historical trading data from Hyperliquid

## Data Used

### Market Sentiment Dataset
Contains daily Bitcoin sentiment classification such as:
- Fear
- Greed

### Trader Dataset
Contains trade-level information including:
- Account
- Coin
- Trade size (USD and tokens)
- Side (Buy/Sell)
- Timestamp
- Closed PnL
- Fees


## Steps in the Analysis

1. **Data Cleaning**
   - Converted timestamps into datetime format
   - Extracted daily date from timestamps
   - Standardized column names
   - Merged trader data with daily sentiment data

2. **Feature Creation**
   - Created a win/loss indicator using Closed PnL
   - Calculated trade size using USD value
   - Computed daily trade activity

3. **Exploratory Analysis**
   - Compared profitability during Fear vs Greed periods
   - Analyzed trade size distribution
   - Studied long vs short trade behavior
   - Observed trading activity patterns


## Key Insights

- Traders tend to be more profitable during **Greed sentiment periods** compared to Fear periods.
- Trade sizes generally increase when the market sentiment is **Greed**, indicating higher trader confidence.
- Larger trades show higher variability in profits compared to smaller trades.


## Strategy Ideas

- During **Fear sentiment**, traders may reduce trade size to manage risk.
- During **Greed sentiment**, traders may increase trading activity to capture stronger market trends.

---

## Project Structure

trader-sentiment-analysis/

data/ → datasets used for analysis  
notebook/ → Jupyter notebook containing the full analysis  
requirements.txt → required Python libraries  
README.md → project documentation  


