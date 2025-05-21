# 📊 FnQ Induction Task – Mean Reversion Strategy (Track 1)

This repository contains a Mean Reversion trading strategy applied to **Reliance Industries (RELIANCE.NS)** stock. The implementation is part of the FnQ Induction Task and demonstrates data handling, strategy design, and backtesting for Indian equities.

---

## 📌 Problem Statement

Design and backtest a logically sound, risk-managed, and statistically robust trading strategy using Indian OHLCV data. Evaluate its performance using relevant quantitative metrics.

---

## ⚙️ Strategy Overview

The strategy is based on **Bollinger Bands** to capture mean-reverting price behavior:
- **Buy Signal**: Price drops below the lower Bollinger Band
- **Sell Signal**: Price crosses above the 20-day Simple Moving Average (Middle Band)

This strategy assumes prices tend to revert to their mean after extreme movements.

---

## 🧠 Logic Breakdown

| Component        | Description                                  |
|------------------|----------------------------------------------|
| **Stock**         | Reliance Industries (RELIANCE.NS)            |
| **Indicator**     | Bollinger Bands (20-day SMA, ±2 std dev)     |
| **Buy Rule**      | Close price < Lower Band                     |
| **Sell Rule**     | Close price > 20-day SMA                     |
| **Capital**       | ₹1,00,000 initial capital                    |
| **Position Size** | Floor division of capital by entry price     |
| **Execution**     | Entry/Exit at next day open                  |

---

## 📈 Backtest Results

- **Final Portfolio Value**: ₹1,15,737
- **Cumulative Return**: +15.7%
- **Number of Trades**: 27
- **Win Rate**: 56%
- **Average Holding Period**: Varies (based on signal)

> Note: Sharpe Ratio, Max Drawdown, and Sortino Ratio can be added in future versions.

---

## 📊 Visualizations

- ✅ Portfolio Equity Curve
- ✅ Bollinger Bands with trade signals
- ⬜ Drawdown and Sharpe not yet implemented

---



