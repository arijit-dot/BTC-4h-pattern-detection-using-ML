# ML-Augmented BTC Pattern Trading Strategy

**A quant-grade system** that boosts traditional candlestick patterns with ML, achieving **3.8 Sharpe** and **60.1% win rate** on BTC/USDT 4H data.

- **SHAP-Explained Decisions**: Volume spikes and ATR ratios drove 70% of model predictions.  
- **Walk-Forward Validated**: Non-overlapping folds (2y train → 90d test) prove robustness.  
- **Crypto-Tuned Risk**: 1% capital risk/trade, 0.1% slippage, and 10% exposure caps.  

**Key Results (2018-2024 Backtest):**
| Metric          | ML Filtered       | Raw Patterns (No ML) |
|-----------------|------------------|----------------------|
| **CAGR**        | 13.7%            | -18.4%               |
| **Sharpe**      | 3.8              | 0.27                 |
| **Max DD**      | -3.8%            | -93.9%               |
| **Win Rate**    | 60.1%            | 52.0%                |

---

🛠️ **Tech Stack**  
```python
Model: RandomForestClassifier(n_estimators=200, class_weight='balanced')  
Features: ['sma50_diff', 'atr_ratio', 'liq_sweep', 'rsi', ...]  
Validation: Walk-forward (2018-2024, 7 folds)  
Backtest: Backtrader with Binance-compatible slippage  







