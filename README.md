# Econ 148 — Project 3: GDP Nowcasting from Mixed-Frequency Indicators
**Track A | Spring 2026 | UC Berkeley**

## Group Members
| Name | 
|------|
| [Nathan Yue ] | 
| [Brandon Lee] |

## Project Overview
We nowcast current-quarter US real GDP growth using monthly and weekly
indicators from FRED released before the BEA advance estimate. We compare
an OLS bridge equation baseline against Ridge/LASSO and gradient boosting,
and benchmark against the Atlanta Fed GDPNow and NY Fed Staff Nowcast.


## Repository Structure
```
├── README.md
├── data/
│   ├── raw/
│   ├── processed/
│   └── external/
├── notebooks/
│   ├── 01_data_collection.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_baseline_model.ipynb
│   └── 04_ml_comparison.ipynb
├── scripts/
│   ├── fetch_fred_data.py
│   ├── clean_series.py
│   ├── build_features.py
│   ├── baseline_models.py
│   └── ml_models.py
├── reports/
│   ├── figures/
│   ├── tables/
│   └── final_report.tex
└── requirements.txt

```

## Data Sources
- **FRED API** (fredapi): GDP, PAYEMS, INDPRO, RSAFS, UMCSENT, UNRATE, GS10, CPIAUCSL, ICSA
- **Atlanta Fed GDPNow**: https://www.atlantafed.org/research-and-data/data/gdpnow
- **NY Fed Staff Nowcast**: https://www.newyorkfed.org/research/policy/nowcast

## Reference Papers
- Fed IFDP 1385 — Dynamic factor model for US GDP nowcasting
- UNCTAD LSTM — LSTM networks applied to nowcasting
- Hopp (2023) — Benchmarking econometric and ML methods for GDP nowcasting
