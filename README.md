# Trader Behavior vs. Market Sentiment Analysis

## Overview
This project is my take on analyzing how a specific crypto trader performs under different market conditions (specifically Bitcoin's Fear & Greed Index). I wanted to dig into the data to see if there were any actionable patterns—essentially, *when should we follow this trader, and when should we fade them?*

## What's Inside?
*   **`analysis.ipynb`**: The main Jupyter Notebook where I cleaned the data, ran the numbers, and visualized the results.
*   **Datasets**: (Not included in repo for privacy/size reasons, but the code expects `historical_data.csv` and `fear_greed_index.csv`).

## Key Findings
After analyzing over 200,000 trades, I found some pretty strong signals:
1.  **Bull Market Sniper**: This trader has an **89% Win Rate** during "Extreme Greed" market conditions. They are exceptional at riding momentum.
2.  **Bear Market Struggles**: Their edge significantly deteriorates during "Extreme Fear", with win rates dropping and average profit per trade halving.
3.  **The Strategy**: My recommendation is to increase position size when the Fear & Greed Index is > 75, and reduce exposure significantly when it drops below 25.

## How to Run it
1.  Clone the repo.
2.  Make sure you have the csv files in the root folder.
3.  Install dependencies: `pip install pandas matplotlib seaborn jupyter`
4.  Run the notebook: `jupyter notebook analysis.ipynb`

---
*Created as part of the data science application process.*
