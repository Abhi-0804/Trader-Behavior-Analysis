# Trader-Behavior-Submission




## Contents
- `Trader_Behavior_Insights.ipynb` — Jupyter notebook with the full analysis pipeline (load, clean, feature engineering, EDA, hypothesis tests, basic regression, and visualization). Ready to run and reproduce results.
- `daily_aggregates.csv` — Daily aggregated metrics (total/avg/median PnL, trade counts, win rate) merged with Fear & Greed data.
- `account_daily_aggregates.csv` — Per-account, per-day aggregates (account_total_pnl, account_trade_count, account_win_rate) merged with sentiment.
- `boxplot_pnl_by_sentiment.png` — Boxplot of account total PnL grouped by sentiment label.
- `rolling_corr.png` — 30-day rolling correlation between total daily PnL and sentiment score.
- `analysis_summary.txt` — Short text summary with quick test results (Kruskal-Wallis and OLS snippet).

## How to use
1. Download and unzip the package.
2. Open `Trader_Behavior_Insights.ipynb` in JupyterLab/Notebook or VS Code and run the cells top-to-bottom. The notebook references the included CSVs in the same folder.
3. If you want to re-run the analysis on new data, replace the CSVs and update the file paths in the first code cell.

## Notes & next steps (suggested)
- Run extended analyses: panel regressions with account fixed effects, logistic models for win probability, lagged sentiment effects, subgroup (by coin/leverage), and backtest simple risk rules (e.g., reduce leverage during Fear).
- I can produce a 1-page executive summary PDF and a 3-slide deck if you want to include a more polished submission for the hiring email.




Files added: Executive_Summary.pdf, Executive_Deck.pptx, daily_aggregates_enhanced.csv, coin_stats_sample.csv
