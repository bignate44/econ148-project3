# Econ 148 — Project 3: GDP Nowcasting from Mixed-Frequency Indicators
**Track A | Spring 2026 | UC Berkeley**

## Group Members
| Name | Role |
|------|------|
| [Name 1] | Group Leader — Data, FRED API, EDA |
| [Name 2] | Modeler — ML training and evaluation |
| [Name 3] | Writer — LaTeX write-up, interpretation |
| [Name 4] | Reviewer — Code review, reproducibility |
| [Name 5] | AI Documenter — AI use documentation |

## Project Overview
We nowcast current-quarter US real GDP growth using monthly and weekly
indicators from FRED released before the BEA advance estimate. We compare
an OLS bridge equation baseline against Ridge/LASSO and gradient boosting,
and benchmark against the Atlanta Fed GDPNow and NY Fed Staff Nowcast.

## How to Reproduce
1. Open `notebooks/gdp_nowcasting.ipynb` in Google Colab
2. Add your FRED API key where indicated at the top of the notebook
3. Click **Runtime → Run All**
4. All data is pulled from the FRED API at runtime — no manual downloads needed

## Repository Structure
```
econ148-project3/
├── notebooks/
│   └── gdp_nowcasting.ipynb   # Main analysis notebook
├── data/
│   └── README.md              # Data sources and notes
├── writeup/
│   ├── checkpoint1.tex        # LaTeX source
│   └── checkpoint1.pdf        # Compiled PDF
└── README.md                  # This file
```

## Data Sources
- **FRED API** (fredapi): GDP, PAYEMS, INDPRO, RSAFS, UMCSENT, UNRATE, GS10, CPIAUCSL, ICSA
- **Atlanta Fed GDPNow**: https://www.atlantafed.org/research-and-data/data/gdpnow
- **NY Fed Staff Nowcast**: https://www.newyorkfed.org/research/policy/nowcast

## Reference Papers
- Fed IFDP 1385 — Dynamic factor model for US GDP nowcasting
- UNCTAD LSTM — LSTM networks applied to nowcasting
- Hopp (2023) — Benchmarking econometric and ML methods for GDP nowcasting
