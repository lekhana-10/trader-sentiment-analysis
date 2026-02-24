# Trader Behavior vs Bitcoin Market Sentiment

## Objective
The objective of this project is to analyze how trader behavior and performance
change across different Bitcoin market sentiment regimes (Fear, Greed, Extreme Greed,
and Neutral) using historical trade data and the Fear & Greed Index.

---

## Datasets
- **fear_greed_index.csv**  
  Contains daily Bitcoin market sentiment classifications.
- **historical_data.csv**  
  Contains trade-level execution details and realized profit/loss information.

---

## Data Availability Note

The historical trade dataset is large and exceeds GitHub's file size limits.
Therefore, it is not included directly in this repository.

link: https://drive.google.com/drive/folders/1-7w7fm5E6dpHmm45ZIysiXBVa7XWXHNX?usp=sharing
To reproduce the analysis:
1. Download the datasets from the provided links in the assignment
2. Place them inside a `data/` folder in the project root
3. Run the notebook from top to bottom

---

## Tools & Libraries
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

---

## Methodology
1. Loaded and inspected both datasets for structure, missing values, and duplicates.
2. Converted trade timestamps to daily granularity for alignment with sentiment data.
3. Resolved date format mismatches to ensure correct dataset merging.
4. Merged trade data with sentiment data using the trading date as the key.
5. Engineered key metrics such as win rate, daily PnL, trade frequency,
   and long vs short behavior.
6. Analyzed trader behavior and performance across sentiment regimes.

---

## Key Insights
- Trading activity is highest during Fear regimes, indicating increased volatility
  and reactive trading behavior.
- Greed and Extreme Greed regimes are dominated by SELL trades, suggesting
  profit-taking behavior.
- Neutral sentiment periods show balanced BUY and SELL activity with lower
  overall trade volume.

---

## Strategy Recommendations
- Apply stricter risk management during Fear regimes due to high volatility.
- Use Greed and Extreme Greed periods as potential profit-taking signals.

---

## How to Run
1. Clone or download this repository.
2. Install required libraries: