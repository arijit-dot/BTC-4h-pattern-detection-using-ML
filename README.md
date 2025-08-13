# ML-Augmented BTC Pattern Trading Strategy

A quant-grade trading system that combines traditional candlestick pattern detection with machine learning to filter high-probability setups. Designed for the BTC/USDT 4H market, with rigorous walk-forward validation and realistic trading constraints.

**Key Results (2018-2024 Backtest):**
| Metric          | ML Filtered       | Raw Patterns (No ML) |
|-----------------|------------------|----------------------|
| **CAGR**        | 13.7%            | -18.4%               |
| **Sharpe**      | 3.8              | 0.27                 |
| **Max DD**      | -3.8%            | -93.9%               |
| **Win Rate**    | 60.1%            | 52.0%                |

![Equity Curve](images/equity curve.png) *(Example plot - replace with your results)*

---

## 🛠️ Features
- **Pattern Detection:** Identifies double/triple tops/bottoms with liquidity sweeps.
- **ML Filter:** Random Forest classifier (SHAP explainability) to score pattern quality.
- **Quant-Grade Backtesting:** 
  - Walk-forward validation (non-overlapping folds).
  - Realistic slippage (0.1%), commissions (0.1%), and risk controls (1% risk/trade).


--
2. Performance Comparison Methodology
Baseline vs. ML-Augmented:
Metric	Raw Patterns (No ML)	ML Filtered (Prob > 0.6)
Total Return	0.1994 (80% loss)	1.1349 (13.5% gain)
CAGR	-18.4%	+13.7%
Sharpe	0.27 (noise-like)	3.8 (professional-grade)
Max DD	-93.9% (near-total wipeout)	-3.8% (low risk)




