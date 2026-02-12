# Fear vs Greed Market Sentiment vs Trader Behavior Analysis

## Project Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed Index)
influences:

-   Trader profitability\
-   Trading frequency\
-   Position sizing\
-   Risk exposure\
-   Behavioral segmentation

It also includes: - A simple next-day profitability check\
- Trader clustering into behavioral archetypes\
- Business-focused strategic insights

The goal is to evaluate whether sentiment drives performance or
primarily affects behavior.

------------------------------------------------------------------------

## Key Questions Answered

1.  Does trader profitability differ between Fear and Greed regimes?
2.  Do traders change behavior based on sentiment?
3.  Can sentiment predict next-day profitability?
4.  Do traders cluster into distinct behavioral archetypes?
5.  What strategic insights can management derive?

------------------------------------------------------------------------

## Project Structure

    Fear_Greed_Trading_Analysis/
    │
    ├── Fear Greed Trading Analysis.py
    ├── fear_greed_index.csv
    ├── historical_data.csv
    ├── README.md
    └── output_plots/

------------------------------------------------------------------------

## Requirements

This project uses only:

-   numpy\
-   pandas\
-   matplotlib\
-   seaborn

Install dependencies:

    pip install numpy pandas matplotlib seaborn

------------------------------------------------------------------------

## Dataset Requirements

### 1) Fear & Greed Index

Required columns: - timestamp - value - classification - date

### 2) Historical Trader Data

Required columns include: - Account - Execution Price - Size USD -
Timestamp IST - Closed PnL

------------------------------------------------------------------------

## Setup Instructions

### Step 1: Clone Repository

    git clone https://github.com/yourusername/fear-greed-trading-analysis.git
    cd fear-greed-trading-analysis

### Step 2: Place Datasets

Place both CSV files in the project directory:

    fear_greed_index.csv
    historical_data.csv

OR update file paths inside the script:

``` python
fear_path = "path/to/fear_greed_index.csv"
trader_path = "path/to/historical_data.csv"
```

------------------------------------------------------------------------

## How to Run

From terminal:

    python "Fear Greed Trading Analysis.py"

The script will:

-   Load & clean datasets\
-   Align sentiment with trading data\
-   Compute daily metrics\
-   Generate visualizations\
-   Perform predictive probability check\
-   Perform trader clustering\
-   Print business-level insights

------------------------------------------------------------------------

## Output Generated

### Console Output Includes:

-   Regime summary statistics\
-   Median PnL comparison\
-   Win rate comparison\
-   Trade frequency comparison\
-   Risk exposure proxy\
-   Predictive probability check\
-   Trader cluster counts\
-   Executive insights

### Visualizations Generated:

-   PnL Distribution by Sentiment\
-   Trade Frequency by Sentiment\
-   Position Size by Sentiment\
-   Risk (Absolute PnL) by Sentiment\
-   Time-series median PnL\
-   Trader Archetype Scatter Plot

------------------------------------------------------------------------

## Key Findings

-   Traders trade more frequently during Fear.\
-   Traders increase position size during Greed.\
-   Risk exposure is higher during Fear.\
-   Profitability difference between regimes is modest.\
-   Sentiment alone has weak predictive power.\
-   Traders cluster into distinct behavioral archetypes.

------------------------------------------------------------------------

## Business Implications

-   Sentiment affects behavior more than edge.\
-   Risk management should be regime-aware.\
-   Segmentation enables differentiated leverage policies.\
-   Sentiment should be used as risk context, not alpha signal.

------------------------------------------------------------------------

## Methodology

-   Daily aggregation per account\
-   Median-based metrics to reduce outlier bias\
-   Absolute PnL used as volatility proxy\
-   Simple probability-based next-day profitability check\
-   K-means clustering using numpy\
-   Overlapping period alignment only

------------------------------------------------------------------------

## Future Improvements

-   Logistic regression model for predictive accuracy\
-   Regime-based Sharpe ratio comparison\
-   Drawdown analysis\
-   Multi-asset comparison\
-   Feature engineering with volatility index

------------------------------------------------------------------------

