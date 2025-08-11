# BTC-4h-pattern-detection-using-ML
This project implements a quantitative trading pipeline for BTC/USDT using pattern detection, machine learning filtering, and backtesting. It detects Double Bottom, Double Top, Triple Bottom, and Triple Top patterns, confirmed by liquidity sweeps, then applies Machine Learning to filter low-probability trades.
🔍 Features
Pattern Detection

Double Bottom & Double Top

Triple Bottom & Triple Top

Liquidity sweep detection for entry confirmation

Trend Filtering

Daily uptrend/downtrend confirmation using moving averages

ML Filtering

Uses Random Forest to predict the probability of a profitable trade

Features include SMA differences, RSI, ATR ratio, MACD-like metrics, ADX proxy, and volume ratios

Backtesting

Walk-forward validation to avoid lookahead bias

Position sizing and exposure control

Performance metrics: Total Return, CAGR, Win Rate, Sharpe Ratio, Max Drawdown

Comparison between ML-filtered strategy and pure pattern-based strategy

📂 Dataset
Source: Binance BTCUSDT 4H OHLCV data (Binance_BTCUSDT_4h_from_1h.csv)

Columns: date, open, high, low, close, volume_btc, tradecount

🚀 How It Works
Data Preparation – Calculates trend indicators and normalizes features

Pattern Detection – Finds reversal patterns & liquidity sweeps

Feature Engineering – Creates technical features for ML model

ML Filtering – Predicts success probability of patterns

Backtest – Runs trades with ML-filtered signals and records performance

📊 Example Results
ML-Filtered Strategy

CAGR: ~13.7%

Win Rate: ~60%

Max Drawdown: ~3.8%

Sharpe Ratio: ~3.80

Pattern-Only Strategy

CAGR: Negative



