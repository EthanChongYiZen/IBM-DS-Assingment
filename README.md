# Extracting and Visualizing Stock Data

Final assignment for the IBM Data Science course (Python for Data Science, AI & Development — PY0220EN). This project extracts historical stock prices and revenue data for Tesla and GameStop, then visualizes both as interactive dashboards.

## Overview

Stock data is pulled via the `yfinance` API and revenue data is scraped from web sources using `BeautifulSoup`. Both datasets are then plotted side-by-side using Plotly — share price on top, quarterly revenue below — with an interactive date range slider.

## Tech Stack

- Python 3.12
- yfinance
- pandas
- requests
- BeautifulSoup (bs4)
- Plotly

## Getting Started

**Install dependencies**

```bash
pip install yfinance bs4 nbformat plotly
```

**Run the notebook**

Open `Final_Assignment__1_.ipynb` in Jupyter and run all cells from top to bottom.

## Notebook Structure

| Question | Description |
|----------|-------------|
| Q1 | Extract Tesla stock data via `yfinance` (ticker: `TSLA`) |
| Q2 | Scrape Tesla quarterly revenue data via BeautifulSoup |
| Q3 | Extract GameStop stock data via `yfinance` (ticker: `GME`) |
| Q4 | Scrape GameStop quarterly revenue data via BeautifulSoup |
| Q5 | Plot Tesla stock price vs. revenue dashboard |
| Q6 | Plot GameStop stock price vs. revenue dashboard |

## Output

Each dashboard displays two interactive charts:
- **Historical Share Price** — closing price over time (up to June 2021)
- **Historical Revenue** — quarterly revenue in USD millions (up to April 2021)

Both charts share an x-axis with a range slider for easy navigation.

## Notes

- This is a course assignment completed as part of the IBM Data Science Professional Certificate on Coursera
- Data is fetched live via `yfinance` and web scraping — results may vary depending on source availability
- Course authored by Joseph Santarcangelo (IBM) and Azim Hirjani
