# 📊 FnQ Induction Task – Mean Reversion Strategy (Track 1)

This project implements a **Mean Reversion Trading Strategy** using OHLCV data for **Reliance Industries (RELIANCE.NS)**. It was developed for the FnQ Induction Task to demonstrate knowledge of trading systems, quantitative analysis, and risk management.

---

## 📌 Problem Statement

Design and backtest a statistically robust, risk-managed trading strategy using Indian equity data. The strategy should be:
- Logically sound
- Well-structured
- Thoroughly documented
- Evaluated using proper performance metrics

---

## ⚙️ Strategy Overview

We use a **Bollinger Bands-based Mean Reversion Strategy**:
- **Buy Signal:** Price crosses below the lower Bollinger Band
- **Sell Signal:** Price crosses back above the 20-day Simple Moving Average (SMA)
- Includes basic volatility filtering and avoids low-volume environments

---

## 🧠 Logic Breakdown

| Component          | Description |
|-------------------|-------------|
| **Indicator**      | Bollinger Bands (20-day SMA, ±2 std dev) |
| **Entry Rule**     | Close price < Lower Bollinger Band |
| **Exit Rule**      | Close price > Middle Band (SMA) |
| **Position Size**  | Fixed capital per trade (no leverage) |
| **Backtest Logic** | Buy/Sell on next day open after signal |

---

## 🗂️ Folder Structure

```
FnQ-MeanReversion-Strategy/
├── data/                   # Raw OHLCV data for Reliance
├── notebooks/              # Jupyter notebook with strategy implementation
├── reports/                # PDF technical report with charts and analysis
├── results/                # Equity curve, drawdown plots, trade charts
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── .gitignore              # Common exclusions
```

---

## 📈 Performance Metrics

| Metric              | Description |
|---------------------|-------------|
| **Cumulative Return**   | Total return over the period |
| **Annualized Return**   | Annualized equivalent of total return |
| **Sharpe Ratio**        | Risk-adjusted return vs volatility |
| **Sortino Ratio**       | Downside-risk-adjusted return |
| **Max Drawdown**        | Largest portfolio loss from peak |
| **Win Rate**            | % of profitable trades |
| **Profit Factor**       | Total profit / total loss |
| **Benchmark Comparison**| NIFTY50 or SENSEX comparison |

(*Calculated in the notebook*)

---

## 📊 Visualizations
- ✅ Price chart with Bollinger Bands & trades
- ✅ Equity curve
- ✅ Drawdown plot
- ✅ Rolling Sharpe ratio (optional)

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```
   notebooks/mean_reversion_strategy.ipynb
   ```

---

## 📚 Resources Used
- [Investopedia – Bollinger Bands](https://www.investopedia.com/terms/b/bollingerbands.asp)
- [Yahoo Finance API via yfinance](https://pypi.org/project/yfinance/)
- FnQ Induction Task PDF

---

## 👤 Author

*Your Name Here*  
IIM/College Name, Year  
[GitHub Profile](https://github.com/yourusername)

---

## ✅ Status

🎯 Final Submission Ready – Includes Code, Report, Metrics & Visuals
