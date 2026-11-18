# Global Air Pollution Analysis

A data project that collects live air-quality readings for cities around the world and explores PM2.5 levels, with the results shown in a Tableau dashboard.

## What it does

- `Pollution_Analysis.py` calls the [World Air Quality Index (WAQI) API](https://aqicn.org/api/) for a list of major cities and monitoring stations on every continent and saves AQI, PM2.5, PM10 and NO2 readings to a CSV file.
- `WAQI dataset - Sheet1.csv` is the collected data: about 300 readings taken in April 2025.
- `Analysis.py` loads the CSV and prints a first look at it: column types, summary statistics and missing values.
- The data is visualised in Tableau: [interactive dashboard](https://public.tableau.com/views/presentpollutionAnalysis/Dashboard1).
- `ReadMe.txt` holds the original project plan (objectives, cleaning steps, EDA ideas).

## Tech

Python 3, requests, pandas, Tableau Public

## How to run

```bash
pip install requests pandas
```

1. Get a free API token from <https://aqicn.org/data-platform/token/>.
2. Put it in `API_KEY` near the top of `Pollution_Analysis.py`. Don't commit your real token.
3. Run `python Pollution_Analysis.py` to collect fresh data, or `python Analysis.py` to explore the included CSV.

## Results

The findings are presented in the Tableau dashboard linked above.
