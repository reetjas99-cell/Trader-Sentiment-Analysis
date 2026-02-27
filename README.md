# Trader-Sentiment-Analysis
Analysis of trader performance vs market sentiment (Fear vs Greed)
Overview
This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance on Hyperliquid. The objective is to identify behavioral patterns, risk tendencies, and performance differences across sentiment regimes and translate them into practical trading insights.
The analysis combines market sentiment data with historical trader execution data to evaluate how trading decisions and outcomes vary under different emotional market conditions.

Objective
The goal of this study is to examine:
Whether trader profitability differs between Fear and Greed markets
How trader behavior (position sizing, trade frequency) changes with sentiment
Which types of traders demonstrate more consistent performance
What actionable risk-management strategies can be derived from observed patterns

Datasets Used
1. Bitcoin Market Sentiment Dataset
Contains daily sentiment classification (Fear, Extreme Fear, Greed, etc.) along with corresponding dates.
Key fields:
date
classification
sentiment value

2. Hyperliquid Historical Trader Dataset
Contains detailed trade-level execution data.
Key fields:
Account
Execution price
Size (USD)
Side (Buy/Sell)
Timestamp
Closed PnL
Fee
Transaction details

Methodology
Data Preparation
Cleaned both datasets and handled missing values
Converted timestamps to daily format for alignment
Merged sentiment data with trading activity on date level
Ensured numeric conversion of PnL and position size fields
Feature Engineering
Key metrics derived for analysis:
Daily PnL per trader
Profitability indicator (win/loss)
Trade frequency per day
Position size trends
Sentiment-wise performance distribution
Segmentation
To better understand behavioral patterns, traders were grouped into:
Frequent vs casual traders (based on trade count)
Profitability consistency patterns
Position size–based behavioral differences

Key Insights
1. Sentiment influences trading behavior more than profitability
Trade frequency and position sizes tend to increase during Greed periods, indicating higher risk appetite. However, higher activity does not consistently translate into higher profitability.

2. Fear-driven markets show higher volatility in outcomes
PnL distributions during Fear phases are more dispersed and unstable, suggesting reactive decision-making and reduced consistency in trading performance.

3. Consistency is linked to controlled position sizing
Traders with relatively stable position sizes and disciplined trade frequency demonstrate more consistent performance compared to highly aggressive participants.

Strategy Implications
Based on observed patterns:
Risk Management During Fear
Reduce position sizing
Focus on capital preservation
Avoid excessive trade frequency
Discipline During Greed
Prevent overexposure from large positions
Maintain structured risk controls
Avoid overconfidence-driven trades
Optimal Trading Behavior
Consistent position sizing
Moderate risk exposure
Systematic execution rather than sentiment-driven decisions

Files in Repository
ASSIGNMENT_NOTEBOOK.ipynb → Complete analysis notebook with charts and modeling
README.md → Project documentation
insights_summary.pdf → One-page summary of findings and strategy recommendations

How to Run
Download datasets
Place CSV files in same folder as notebook
Open notebook in Jupyter/Colab
Run all cells sequentially

Dependencies:
pandas
matplotlib
seaborn
scikit-learn

Conclusion
This analysis demonstrates that while market sentiment alone does not determine profitability, it significantly affects trader behavior and risk-taking patterns. Traders maintaining disciplined execution and controlled exposure across sentiment regimes show more stable performance outcomes.

Understanding sentiment-driven behavioral shifts can help design more robust and risk-aware trading strategies.
