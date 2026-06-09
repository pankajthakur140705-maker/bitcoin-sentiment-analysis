# Bitcoin Market Sentiment vs Trader Performance Analysis

## Executive Summary

This project investigates the relationship between Bitcoin market sentiment and trader performance using historical trading data from Hyperliquid and the Bitcoin Fear & Greed Index.

By integrating sentiment indicators with trading activity, the analysis aims to identify behavioral patterns, evaluate trader profitability across different market conditions, and generate insights that can support data-driven trading strategies.

---

## Problem Statement

Market sentiment plays a significant role in financial markets, particularly in cryptocurrency trading where investor psychology often drives short-term price movements.

The objective of this study is to determine:

* How trader profitability varies across different sentiment regimes.
* Whether Fear or Greed conditions lead to better trading outcomes.
* How market psychology influences trading behavior and risk-taking.

---

## Data Sources

### Bitcoin Fear & Greed Index

Daily sentiment data representing market psychology.

Attributes:

* Date
* Sentiment Value
* Classification

  * Extreme Fear
  * Fear
  * Neutral
  * Greed
  * Extreme Greed

### Hyperliquid Historical Trader Dataset

Transaction-level trading records containing:

* Account Information
* Coin/Symbol
* Trade Side
* Execution Price
* Position Size
* Leverage
* Closed PnL
* Fees
* Trade Timestamp

---

## Methodology

### Data Preparation

* Loaded datasets using Pandas.
* Converted timestamp fields into datetime format.
* Standardized date formats.
* Merged datasets on trading date.

### Exploratory Data Analysis

The following metrics were analyzed:

* Average Closed PnL
* Trading Volume
* Win Rate
* Sentiment Distribution
* Trader Performance Trends

### Visualization

Visualizations were generated to evaluate:

* Profitability by Sentiment
* Win Rate by Sentiment
* Trading Activity by Sentiment

---

## Key Insights

### 1. Market Sentiment Impacts Profitability

Analysis indicates that trader profitability differs significantly across sentiment categories.

Fear-driven market conditions produced stronger average returns compared to highly optimistic market environments.

### 2. Extreme Greed Shows Lower Performance

Performance declined during periods classified as Extreme Greed, suggesting possible overconfidence and increased risk exposure among market participants.

### 3. Sentiment as a Trading Signal

The results suggest that sentiment indicators can provide additional context for identifying favorable market conditions and improving risk management decisions.

---

## Business Value

The findings demonstrate how alternative data sources such as market sentiment can enhance quantitative trading workflows.

Potential applications include:

* Risk Management
* Strategy Optimization
* Market Timing
* Behavioral Finance Analysis
* Algorithmic Trading Research

---

## Technology Stack

| Category                | Tools                          |
| ----------------------- | ------------------------------ |
| Programming Language    | Python                         |
| Data Processing         | Pandas, NumPy                  |
| Visualization           | Matplotlib, Seaborn            |
| Development Environment | Jupyter Notebook, Google Colab |
| Version Control         | Git, GitHub                    |

---

## Repository Structure

```text
bitcoin-sentiment-analysis/
│
├── notebook/
│   └── analysis.ipynb
│
├── report/
│   └── report.md
│
├── images/
│   ├── avg_pnl_by_sentiment.png
│   ├── win_rate_by_sentiment.png
│   └── trading_volume_by_sentiment.png
│
├── requirements.txt
└── README.md
```

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Running the Project

1. Clone the repository.
2. Install dependencies.
3. Open the notebook located in the notebook directory.
4. Execute all cells sequentially.

```bash
git clone <repository-url>
cd bitcoin-sentiment-analysis
jupyter notebook
```

---

## Results

The analysis confirms a measurable relationship between Bitcoin market sentiment and trader performance.

Key observations indicate that:

* Fear and Extreme Fear periods generated stronger average profitability.
* Sentiment influences trader behavior and market participation.
* Incorporating sentiment indicators can improve trading decision-making frameworks.

---

## Future Improvements

* Machine Learning-based Profitability Prediction
* Time-Series Forecasting Models
* Real-Time Sentiment Integration
* Advanced Trader Segmentation
* Portfolio Risk Analysis

---

## Author

**Pankaj Thakur**

B.Tech – Computer Science Engineering
Government Hydro Engineering College (GHEC)

---

## License

This project was developed as part of a Data Science internship assessment and is intended for educational and research purposes.
