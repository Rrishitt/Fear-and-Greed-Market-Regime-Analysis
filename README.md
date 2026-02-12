Fear vs Greed Market Sentiment vs Trader Behavior Analysis
Project Overview

This project analyzes how Bitcoin market sentiment (Fear vs Greed Index) influences:

Trader profitability

Trading frequency

Position sizing

Risk exposure

Behavioral segmentation

It also includes:

A simple next-day profitability check

Trader clustering into behavioral archetypes

Business-focused strategic insights

The goal is to evaluate whether sentiment drives trading performance or primarily affects trader behavior.

Key Questions Answered

Does trader profitability differ between Fear and Greed regimes?

Do traders change behavior based on sentiment?

Can sentiment predict next-day profitability?

Do traders cluster into distinct behavioral archetypes?

What strategic insights can management derive?

Project Structure
Fear_Greed_Trading_Analysis/
│
├── Fear Greed Trading Analysis.py
├── fear_greed_index.csv
├── historical_data.csv
├── README.md
└── output_plots/

Requirements

This project uses only:

numpy

pandas

matplotlib

seaborn

Install dependencies:

pip install numpy pandas matplotlib seaborn

Dataset Requirements
1) Fear & Greed Index

Required columns:

timestamp

value

classification

date

2) Historical Trader Data

Required columns include:

Account

Execution Price

Size USD

Timestamp IST

Closed PnL

Setup Instructions
Step 1: Clone Repository
git clone https://github.com/yourusername/fear-greed-trading-analysis.git
cd fear-greed-trading-analysis

Step 2: Place Datasets

Place both CSV files in the project directory:

fear_greed_index.csv
historical_data.csv


OR update file paths inside the script:

fear_path = "path/to/fear_greed_index.csv"
trader_path = "path/to/historical_data.csv"

How to Run

From the terminal:

python "Fear Greed Trading Analysis.py"


The script will:

Load and clean datasets

Align sentiment with trading data

Compute daily account-level metrics

Generate visualizations

Perform predictive probability check

Perform trader clustering

Print business-level insights

Output Generated
Console Output Includes

Regime summary statistics

Median PnL comparison

Win rate comparison

Trade frequency comparison

Risk exposure proxy

Predictive probability check

Trader cluster counts

Executive-level insights

Visualizations Generated

PnL Distribution by Sentiment

Trade Frequency by Sentiment

Position Size by Sentiment

Risk (Absolute PnL) by Sentiment

Time-series median PnL

Trader Archetype Scatter Plot

Key Findings

Traders trade more frequently during Fear regimes.

Traders increase position size during Greed regimes.

Risk exposure is higher during Fear periods.

Profitability differences between regimes are modest.

Sentiment alone has weak predictive power.

Traders cluster into distinct behavioral archetypes.

Business Implications

Sentiment affects trading behavior more than profitability.

Risk management should be regime-aware.

Behavioral segmentation enables differentiated leverage policies.

Sentiment should be treated as a risk indicator, not an alpha signal.

Methodology

Daily aggregation per account

Median-based metrics to reduce outlier bias

Absolute PnL used as a volatility proxy

Simple probability-based next-day profitability check

K-means clustering implemented using numpy

Strict overlapping-period data alignment
