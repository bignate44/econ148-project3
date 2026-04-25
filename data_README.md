# Data Sources

All data is pulled at runtime from the FRED API using the `fredapi` Python package.
No static data files are stored in this repository.

## FRED Series Used
| Series ID   | Description                        | Frequency |
|-------------|-----------------------------------|-----------|
| GDP         | Real Gross Domestic Product        | Quarterly |
| PAYEMS      | Nonfarm Payrolls                   | Monthly   |
| INDPRO      | Industrial Production Index        | Monthly   |
| RSAFS       | Real Retail Sales                  | Monthly   |
| UMCSENT     | Consumer Sentiment (U of Michigan) | Monthly   |
| UNRATE      | Civilian Unemployment Rate         | Monthly   |
| GS10        | 10-Year Treasury Yield             | Monthly   |
| CPIAUCSL    | CPI All Urban Consumers            | Monthly   |
| ICSA        | Initial Jobless Claims             | Weekly    |

## How to Access
1. Get a free API key at https://fred.stlouisfed.org/docs/api/api_key.html
2. Set `FRED_API_KEY = "your_key_here"` at the top of the notebook
3. Run the notebook — all data downloads automatically

## Benchmark Sources
- Atlanta Fed GDPNow: https://www.atlantafed.org/research-and-data/data/gdpnow
- NY Fed Staff Nowcast: https://www.newyorkfed.org/research/policy/nowcast
