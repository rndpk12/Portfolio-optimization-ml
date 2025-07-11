# Integrated Machine Learning Framework for Portfolio Optimization and Risk Assessment

This project explores **machine learning** and **quantitative optimization** techniques to construct and evaluate five optimized investment portfolios based on **Nifty 50** stock data (2014–2023). It integrates:
- Predictive modeling (XGBoost, GARCH)
- Clustering (Hierarchical Clustering)
- Optimization (Mean-Variance, Hierarchical Risk Parity)

---

## Project Structure

- `portfolio_optimization.ipynb` – Main Jupyter notebook with all model implementations.
- `Report.docx` – Full research paper with detailed explanation and results.
- `data/` – Folder for input stock data (not uploaded due to size).
- `images/` – Folder for all graphs and visuals (add your plots here).

---

##  Methodologies Used

### Portfolio Selection

- Top 25% Stocks by **Sharpe Ratio**
- Top 25% Stocks by **MAPE**
- All Nifty 50 Stocks
- 11 Sectoral Representatives
- Agglomerative Hierarchical Clustering

### Optimization Techniques

- **Mean-Variance Optimization**
- **Monte Carlo Simulation**
- **Hierarchical Risk Parity (HRP)**
- **GARCH Model** for volatility forecasting

---

## Key Results

| Portfolio Strategy                        | Annualized Return | Sharpe Ratio | Max Drawdown | CVaR (95%) |
|------------------------------------------|-------------------|--------------|--------------|------------|
| 11 Stocks from 11 Sectors (MVO)          | 21.3%             | 1.89         | -32.9%       | -2.5%      |
| Top 25% Sharpe Stocks (MVO)              | 20.7%             | 1.88         | -34.7%       | -2.6%      |
| Top 25% Low MAPE Stocks (MVO)            | 21.6%             | 1.01         | -26.8%       | -2.1%      |
| All Nifty 50 (MVO)                       | 23.7%             | 1.38         | -26.3%       | -2.1%      |
| All Nifty 50 (HRP)                       | 21.8%             | **3.26**     | -62.6%       | **-0.1%**  |

>  **Best Sharpe Ratio**: HRP Portfolio  
>  **Best Clamar Ratio**: All Nifty 50 (MVO)  
>  **Best Risk-adjusted Return**: HRP Portfolio
