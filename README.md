# Portfolio Optimization using Monte Carlo Simulation

**Author:** Michael Owen A.  
**Date:** June 2026

## Overview
Modern Portfolio Theory implementation using Python (Jupyter Notebook) to optimize asset allocation and map the Efficient Frontier via 500,000 Monte Carlo simulations.

### Methodology
1. **Data Acquisition**: Fetching historical data from Yahoo Finance for a basket of high-growth assets.
2. **Simulation**: Generating 500,000 random weight allocations using vectorized NumPy operations.
3. **Optimization**: Applying the *Modern Portfolio Theory* (MPT) framework to maximize the Sharpe Ratio.

---

## Mathematical Framework

The simulated portfolios are evaluated using three core metrics:

**1. Expected Portfolio Return**
$$E(R_p) = \sum_{i=1}^{n} w_i E(R_i)$$

**2. Portfolio Volatility**
$$\sigma_p = \sqrt{w^T \Sigma w}$$

**3. Sharpe Ratio**
$$Sharpe = \frac{E(R_p) - R_f}{\sigma_p}$$

---

## Simulation Results & Output

### Console Output Logs
```text
[*********************100%***********************]  7 of 7 completed
Risk Free Rate:  4.38%
Max Sharpe Ratio: 1.2276
Expected Return: 42.31%
Volatility: 30.90%

Optimal Asset Allocation:
AAPL: 0.06%
AMZN: 0.91%
AVGO: 39.64%
BRK-B: 25.83%
GOOG: 4.68%
MSFT: 2.10%
NVDA: 26.78%
