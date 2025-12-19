# TMinus4 — Intraday Quantitative Trading Strategy

## Overview
This project was developed as part of the **Inter IIT Bootcamp (Quant Problem Statement)**.
The objective was to design an intraday trading strategy using only **OHLCV data** on a subset
of **NIFTY 100 stocks**, with all positions closed by day-end.

## Approaches Explored
- Statistical methods using **Auto-Regressive models**, **Ornstein–Uhlenbeck process**, and **Kalman filtering**
- Cross-sectional intraday correlation hypothesis
- **Machine Learning-based strategy (final)** using Random Forest

## Final Strategy (ML-Based)
- Random Forest classifier with **93 momentum-based features**
- Features capture short-term (1–20) and long-term (40–240) momentum
- Trades executed every **15 minutes**
- Top 7 stocks taken **long**, bottom 7 taken **short**
- Intraday square-off to avoid overnight risk

## Results (Backtested)
- **Net Returns:** 517.9%
- **Sharpe Ratio:** 9.19
- **Sortino Ratio:** 13.18
- **Max Drawdown:** 6.64%
- **Number of Trades:** 86,352
- **Winning Trades:** 56.47%

## Repository Structure
- `notebooks/` — Jupyter notebooks for strategy and backtesting
- `report/` — Project report and presentation slides

## Disclaimer
This project is for **academic and research purposes only** and does not constitute financial advice.
