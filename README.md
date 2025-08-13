# ML-Augmented BTC Pattern Trading Strategy

A quant-grade trading system that combines traditional candlestick pattern detection with machine learning to filter high-probability setups. Designed for the BTC/USDT 4H market, with rigorous walk-forward validation and realistic trading constraints.
Model: RandomForestClassifier (scikit-learn)
Validation: Strict walk-forward (2y train → 90d test)

**Key Results (2018-2024 Backtest):**
| Metric          | ML Filtered       | Raw Patterns (No ML) |
|-----------------|------------------|----------------------|
| **CAGR**        | 13.7%            | -18.4%               |
| **Sharpe**      | 3.8              | 0.27                 |
| **Max DD**      | -3.8%            | -93.9%               |
| **Win Rate**    | 60.1%            | 52.0%                |

---

## 🛠️ Features
- **Pattern Detection:** Identifies double/triple tops/bottoms with liquidity sweeps.
- **ML Filter:** Random Forest classifier (SHAP explainability) to score pattern quality.
- **Quant-Grade Backtesting:** 
  - Walk-forward validation (non-overlapping folds).
  - Realistic slippage (0.1%), commissions (0.1%), and risk controls (1% risk/trade).







