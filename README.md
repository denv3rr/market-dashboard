[![Python](https://img.shields.io/badge/python-3.9+-blue)](#)
![Repo Size](https://img.shields.io/github/repo-size/denv3rr/market-dashboard)
![GitHub Created At](https://img.shields.io/github/created-at/denv3rr/market-dashboard)
![Last Commit](https://img.shields.io/github/last-commit/denv3rr/market-dashboard)
![Issues](https://img.shields.io/github/issues/denv3rr/market-dashboard)
![License](https://img.shields.io/github/license/denv3rr/market-dashboard)
![Website](https://img.shields.io/website?url=https%3A%2F%2Fseperet.com&label=seperet.com)

<br>

A lightweight, open-source market analysis dashboard.
Fetches live market data and displays interactive charts with technical indicators.
<br>

> [!NOTE]
>
> Work in progress.

<br><br>

<div>
  <a href="https://seperet.com">
    <img width="100" src=https://github.com/denv3rr/denv3rr/blob/main/IMG_4225.gif/>    
  </a>
</div>

## Features

- Fetch live stock data via Yahoo Finance and Finnhub.io
- Interactive candlestick charts (Plotly)
- Toggle overlays like:
  - 20-day MA (Moving Average)
  - RSI (Relative Strength Index)
- Sidebar input for custom ticker, timeframe, and interval
- Drag/drop-ready preset support (coming soon)

---

## Usage

### 1. Clone the Repo or Download ZIP

```bash
git clone https://github.com/denv3rr/market-dashboard.git
cd MarketDashboard
```

### 2. Install Requirements

- streamlit  
- yfinance  
- plotly  
- pandas
- python-dotenv  
- requests (for Finnhub API)

```bash
pip install -r requirements.txt
```

### 3. Set Up Finnhub.io API Key

To use stock symbol data from [Finnhub](https://finnhub.io):

1. Create a free account at: [https://finnhub.io/register](https://finnhub.io/register)
   
2. Go to your [API dashboard](https://finnhub.io/dashboard) to get your token.
   
3. Add this token to your environment variables or `.env` file (recommended - API keys will not be commited from this file):
   
    ```bash
    export FINNHUB_API_KEY=your_api_key_here
    ```
    
4. Alternatively, update the key directly in `core/api.py` if needed (not recommended - this file is not added to `.gitignore`).

> [!NOTE]
>
> Some international exchanges require a paid plan with Finnhub.

### 4. Launch UI Dashboard

- ```bash
  python app.py
  ```

or

- ```bash
  streamlit run ui/dashboard.py
  ```

Or

- double-click `run_dashboard.bat` (Windows only).

---

<!--
## Roadmap

- Add drawing tools (trend lines, zones)
- Enable backtesting custom strategies
- Import/export preset overlays
- Real-time data streaming (WebSockets)
- Modular quant strategy plugin system

---

## Reminders / To-Do

- Tab auto-close timeout if no confirmation
- Transition/fade animations
- Tab reordering support
- Dark/light mode toggle
- Sidebar hover & dropdown styling polish
- Improve tab confirmation UX (click-away, no flicker)
- Optional logging/export feature (CSV or JSON)

---
-->
