# Optimal Portfolio Allocation and Value at Risk (VaR)

Author: Shota Wada  
Date: June 2023

## Overview

This report presents my analytical and numerical responses to the CQF Part One Exam, focusing on portfolio optimization, risk analysis, and Value at Risk (VaR) backtesting. The exam evaluates a candidate's proficiency in modern quantitative finance techniques including Lagrangian optimization, Sharpe Ratio interpretation, Monte Carlo simulation, and historical risk measures.

## Contents

### Question 1 – Global Minimum Variance Portfolio
- Derives the analytical solution to the Global Minimum Variance (GMV) portfolio.
- Shows the use of Lagrangian multipliers under a budget constraint.
- Includes code in Python using `NumPy`, `SciPy`, and `Pandas`.
- Presents computed optimal weights and portfolio risk.

### Question 2 – Portfolio Optimization with Target Return
- Extends optimization to include a return constraint.
- Uses three scaled correlation matrices (x1, x1.3, x1.8) to examine the impact of correlation on risk.
- Presents a clean result table showing optimal weights and risk per scenario.

### Question 3 – Sharpe Ratio Frequency Effects
- Demonstrates how Sharpe Ratios vary by observation frequency (daily, monthly, quarterly, annual).
- Converts Sharpe Ratios into loss probabilities to highlight perceived risk differences.
- Explains the psychological impact of over-monitoring investments.

### Question 4 – Random Portfolio Simulation
- Simulates 700 random portfolios with standardized weights.
- Computes expected return (μΠ), risk (σΠ), and Sharpe Ratios.
- Visualizes the efficient frontier using `Plotly`.

### Question 5 – Historical VaR Backtesting (99% / 10-Day)
- Uses Nasdaq-100 historical data (2012–2023) to backtest parametric VaR.
- Identifies actual breaches vs. expected breaches.
- Detects market stress events (e.g., COVID-19 crash in 2020).
- Visualizes breaches and returns over time.

### Question 6 – EWMA-Based VaR Backtesting
- Re-implements VaR using Exponentially Weighted Moving Average (EWMA) volatility.
- Initializes using long-term variance, λ = 0.72.
- Compares breach frequency with historical VaR.
- Shows the smoothing effect of high λ values in volatility forecasts.

## Tools Used

- Python 3 (Jupyter Notebook)
- Libraries: `NumPy`, `Pandas`, `SciPy`, `Plotly`, `Matplotlib`
- Data Sources: Simulated data and historical Nasdaq-100 prices

## Files

- `E1_SHOTAWADA_REPORT.pdf` – Full exam report with mathematical derivations, Python code, outputs, and discussion
- `nasdaq100.csv` – Historical dataset used for VaR backtesting (not included here)

## Remarks

- All analytical results avoid excessive reliance on numerical solvers, as per exam guidelines.
- Python code is modular, reproducible, and well-commented for validation.
- The report clearly differentiates between theory, implementation, and interpretation.

---

**Note**: This project is part of the CQF Program and intended for academic and professional assessment purposes only.
