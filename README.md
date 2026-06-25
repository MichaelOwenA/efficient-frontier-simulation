# Portfolio Optimization: Monte Carlo Simulation

**Author:** Michael Owen A.  
**Date:** June 2026

---

## Overview
This project implements **Modern Portfolio Theory (MPT)** to optimize asset allocation. By running 500,000 Monte Carlo simulations, the model identifies the optimal weight distribution that maximizes the Sharpe Ratio, visually represented by the Efficient Frontier.

---

## Simulation Results
The simulation successfully processed the asset basket, identifying a maximum Sharpe Ratio of **1.2276**.

![Efficient Frontier Visualization](efficient_frontier.png)

### Key Performance Metrics
| Metric | Value |
| :--- | :--- |
| **Risk-Free Rate ($R_f$)** | 4.38% |
| **Max Sharpe Ratio** | 1.2276 |
| **Expected Return** | 42.31% |
| **Portfolio Volatility** | 30.90% |

### Optimal Asset Allocation
* **AVGO**: 39.64%
* **NVDA**: 26.78%
* **BRK-B**: 25.83%
* **GOOG**: 4.68%
* **MSFT**: 2.10%
* **AMZN**: 0.91%
* **AAPL**: 0.06%

---

## Mathematical Framework
Portfolios are evaluated based on these core financial metrics:

* **Expected Portfolio Return** $E(R_p)$: The weighted sum of expected individual asset returns.

  $$E(R_p) = \sum_{i=1}^{n} w_i E(R_i)$$

* **Portfolio Volatility** $\sigma_p$: The annualized standard deviation of portfolio returns, reflecting historical asset covariances.

  $$\sigma_p = \sqrt{w^T \Sigma w}$$

* **Sharpe Ratio:** The measure of risk-adjusted performance, quantifying excess return per unit of annualized volatility.

  $$Sharpe = \frac{E(R_p) - R_f}{\sigma_p}$$

---

## Instructions for Execution

### 1. Prerequisites
Ensure you have the following dependencies installed:
```bash
pip install yfinance numpy pandas matplotlib
