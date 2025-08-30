# Online Correlation Changepoint Detection via Adaptive EWMA Charts

This repository contains the code and results for the MSc thesis:

> **Online Correlation Changepoint Detection via Adaptive EWMA Charts**  
> *Jilly Lim — MSc Machine Learning and Data Science (Online), Imperial College London, 2025*

## Project Overview

This project investigates **real-time detection of changes in correlation** between two time series, using rolling Pearson correlation as a test statistic. We propose an **Adaptive EWMA** control chart and compare it against three established methods:

- **CUSUM** – classical mean-shift detector  
- **Wilcoxon Rank-Sum Scan** – nonparametric windowed test  
- **MEWMA** – multivariate EWMA applied to bivariate raw stream  

Both simulated studies and real-world case studies are included:
- Financial data (e.g., NVDA vs GOOGL, Zoom vs S&P 500)
- Public health data (COVID-19 case rates: Los Angeles vs San Francisco)

## Files

| File                  | Description                          |
|-----------------------|--------------------------------------|
| `thesis_clean.ipynb`  | Full code (no output, minimal size)  |
| `thesis_clean.html`   | HTML version of above                |
| `thesis_results.ipynb`| Full code **with all outputs**       |
| `thesis_results.html` | HTML version with outputs            |

Both notebooks contain identical code and analysis; only the presence of outputs differs.


## Notes

- Code is written in Python 3 and intended for reproducibility.
- Datasets are publicly available via Kaggle and are downloaded using `kagglehub`.
- Some sections (e.g., simulation runs) may take several minutes to execute.

## Setup

This project uses standard Python packages including:

- `numpy`, `pandas`, `matplotlib`, `scipy`
- `kagglehub` (for downloading public datasets)

Install with:

```bash
pip install numpy pandas matplotlib scipy kagglehub


