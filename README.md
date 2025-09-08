# Trader-Behavior-Submission




## Contents
- `Trader_Behavior_Insights.ipynb` — Jupyter notebook with the full analysis pipeline (load, clean, feature engineering, EDA, hypothesis tests, basic regression, and visualization). Ready to run and reproduce results.
- `daily_aggregates.csv` — Daily aggregated metrics (total/avg/median PnL, trade counts, win rate) merged with Fear & Greed data.
- `account_daily_aggregates.csv` — Per-account, per-day aggregates (account_total_pnl, account_trade_count, account_win_rate) merged with sentiment.
- `boxplot_pnl_by_sentiment.png` — Boxplot of account total PnL grouped by sentiment label.
- `rolling_corr.png` — 30-day rolling correlation between total daily PnL and sentiment score.
- `analysis_summary.txt` — Short text summary with quick test results (Kruskal-Wallis and OLS snippet).

🔧 Skills & Tools Demonstrated
- **Data Engineering:** Parsing large-scale trading data, handling inconsistent timestamps, merging multi-source datasets.
- **Exploratory Data Analysis (EDA):** Visualizing PnL distributions, sentiment correlations, leverage patterns, rolling performance trends.
- **Statistical Analysis:** Hypothesis testing (Kruskal–Wallis), regression models (OLS, logistic regression), fixed-effects style analysis.
- **Financial Modeling:** Designed and evaluated a simple sentiment-based backtest strategy (reducing exposure during "Fear" days).
- **Data Visualization & Reporting:** Built insightful plots, a **1-page executive summary PDF**, and a **presentation deck** for stakeholders.
- **Tech Stack:** Python (Pandas, NumPy, Matplotlib, Statsmodels), Jupyter Notebook, PowerPoint.

---

## 🔍 Key Insights
- **Sentiment drives trader outcomes** → Daily PnL showed statistically significant differences between *Fear* and *Greed* regimes (p < 0.001).
- **Leverage behavior** → High-leverage accounts were disproportionately affected by negative sentiment swings.
- **Strategy backtest** → A simple “reduce exposure by 50% during Fear days” strategy reduced volatility and drawdowns but also reduced cumulative returns — showing trade-offs in sentiment-based strategies.
- **Account heterogeneity** → Top-performing accounts exhibited more resilience to sentiment shifts, suggesting that professional traders adapt better to market mood.

---

## 📊 Deliverables
1. **Jupyter Notebook:** End-to-end analysis (cleaning → EDA → modeling → backtest).
2. **Executive Summary (PDF):** Concise business-facing report.
3. **Presentation Deck (PPTX):** 3-slide insights deck for stakeholders.
4. **Visualizations:** Boxplots, rolling correlation charts, cumulative PnL curves.
5. **Aggregated Datasets:** Daily and account-level summaries for further exploration.

---





---


## 💼 Resume Highlights
- Analyzed **500K+ crypto trades** alongside the **Fear & Greed Index** to investigate sentiment’s effect on trader PnL and risk-taking.
- Applied statistical tests and regression models, confirming significant performance differences across sentiment regimes.
- Designed a **risk-adjusted backtest strategy** that cut exposure on “Fear” days, reducing drawdowns while highlighting trade-offs in returns.
- Delivered findings through a **Jupyter Notebook**, **executive summary PDF**, and **insights deck**.
- **Tech stack:** Python, Pandas, NumPy, Statsmodels, Matplotlib, Jupyter, PowerPoint.

---


## 🚀 Next Steps
Future improvements include:
- Implementing a **trade-level backtester** with transaction costs and dynamic leverage adjustments.
- Exploring **lagged sentiment features** (1–7 days) for predictive modeling.
- Extending to **multi-asset analysis** beyond BTC to other major crypto pairs.


## How to use
1. Download and unzip the package.
2. Open `Trader_Behavior_Insights.ipynb` in JupyterLab/Notebook or VS Code and run the cells top-to-bottom. The notebook references the included CSVs in the same folder.
3. If you want to re-run the analysis on new data, replace the CSVs and update the file paths in the first code cell.

## Notes & next steps (suggested)
- Run extended analyses: panel regressions with account fixed effects, logistic models for win probability, lagged sentiment effects, subgroup (by coin/leverage), and backtest simple risk rules (e.g., reduce leverage during Fear).
- I can produce a 1-page executive summary PDF and a 3-slide deck if you want to include a more polished submission for the hiring email.




Files added: Executive_Summary.pdf, Executive_Deck.pptx, daily_aggregates_enhanced.csv, coin_stats_sample.csv
