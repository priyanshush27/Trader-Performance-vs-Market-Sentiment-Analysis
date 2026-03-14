# Trader-Performance-vs-Market-Sentiment-Analysis


## Overview
This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance on the Hyperliquid trading platform. The goal is to identify patterns that could inform smarter trading strategies.

The analysis uses two datasets:
1. Bitcoin Fear & Greed Index
2. Historical Hyperliquid trader transaction data

---

## Methodology

The analysis was performed using Python (Pandas, Matplotlib, Seaborn).

### Data Preparation
- Loaded and explored both datasets
- Converted timestamps to daily dates
- Aligned trader activity with market sentiment by merging datasets on date
- Created key metrics including:
  - Daily PnL
  - Win rate
  - Trade frequency
  - Position size (used as a proxy for leverage exposure)

### Behavioral Metrics
Several trader behavior metrics were analyzed:

- Trade frequency
- Position size distribution
- Long vs short bias
- Trader segmentation (frequency, leverage exposure, consistency)

---

## Key Findings

### 1. Market Sentiment Impacts Profitability
Average PnL and win rate are higher during **Greed periods**, suggesting traders perform better when market sentiment is bullish.

### 2. Higher Trading Frequency Reduces Profitability
Infrequent traders achieve the highest average PnL per trade, while frequent traders generate lower average returns. This suggests that excessive trading may reduce trade quality.

### 3. Win Rate Alone Does Not Determine Profitability
Traders with higher win rates do not necessarily generate the highest profits. Profitability appears to depend more on the size of winning trades relative to losses.

---

## Strategy Recommendations

### Strategy 1 — Trade Selectively
Since infrequent traders achieve higher average PnL per trade, traders should prioritize **high-quality trade setups rather than high-frequency trading**.

### Strategy 2 — Adjust Strategy Based on Market Sentiment
Trading performance improves during Greed periods. Traders may benefit from increasing activity during bullish sentiment while being more cautious during Fear periods.

---

## How to Run

1. Clone the repository
2. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn
