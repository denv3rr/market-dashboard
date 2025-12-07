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
- Ticker search, timeframe, and interval sidebar
- Toggle overlays like:
  - 20-day MA (Moving Average)
  - RSI (Relative Strength Index)

---

## Usage

### 1. Clone the Repo or Download ZIP

```bash
git clone https://github.com/denv3rr/market-dashboard.git
cd market-dashboard
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

> [!NOTE]
>
> Although the basic Finnhub.io service is currently free,
> some international exchanges require a paid plan.

#### To use stock symbol data from [Finnhub](https://finnhub.io):

1. Create a free account at: [https://finnhub.io/register](https://finnhub.io/register)
   
2. Then go to your [API dashboard](https://finnhub.io/dashboard) to get your API key/token.

#### Update your `.env.example` file and add your API key

3. Change the file name from `.env.example` to just `.env`
   
4. Add your API key to that `.env` file:
   
    ```bash
    export FINNHUB_API_KEY=your_api_key_here
    ```

> [!WARNING]
>
> Remember not to commit this file if you clone this.

### 4. Launch Dashboard

- ```bash
  python app.py
  ```

or

- ```bash
  streamlit run ui/dashboard.py
  ```

Windows only:

- double-click `run_dashboard.bat` (Windows only).

---
