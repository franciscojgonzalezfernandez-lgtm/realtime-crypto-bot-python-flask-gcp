# Automatic Trading Algorithm - Binance Crypto Bot (2021)

## 🚀 About This Project

**Real-time cryptocurrency trading bot** for Binance API. Features **live trading**, **backtesting strategies**, **Telegram notifications**, **Google BigQuery logging**, and **Data Studio dashboards**. Built in 2021 to test algorithmic trading theories.


## ✨ Tech Stack (2021)

| Category          | Technologies                              |
|-------------------|-------------------------------------------|
| **Framework**     | Flask + Gunicorn                          |
| **Data Analysis** | **Pandas + NumPy + TA-Lib** (indicators)  |
| **Database**      | **Google BigQuery** (trade logs)          |
| **Analytics**     | **Google Data Studio** (dashboards)       |
| **Queue**         | **Google Cloud Tasks**                    |
| **Cache**         | **Redis**                                 |
| **Secrets**       | **Google Secret Manager**                 |
| **Notifications** | **Telegram Bot**                          |
| **Exchange**      | **Binance API** (real-time)               |
| **Visualization** | **Matplotlib**                            |

## 🎯 Core Features

- **Live Trading** - Real-time Binance API operations
- **Backtesting** - Strategy validation with historical data
- **Telegram Alerts** - Entry/exit signals + error monitoring
- **BigQuery Logging** - All trades persisted for analysis
- **Data Studio Dashboards** - Performance visualization
- **Technical Analysis** - TA-Lib indicators (RSI, MACD, etc.)

## 🎯 Trading Workflow

1. Fetch Binance real-time data (WebSocket)

2. Apply TA indicators (Pandas + TA-Lib)

3. Strategy signals → Backtest validation

4. Live trades → Google Tasks queue

5. BigQuery logging + Redis cache

6. Data Studio dashboards + Telegram alerts


## 🎯 Getting Started

```bash
# Clone & Install (Python 3.8+)
git clone https://github.com/franciscojgonzalezfernandez-lgtm/realtime-crypto-bot-python-flask-gcp.git
cd realtime-crypto-bot-python-flask-gcp

# Install dependencies
pip install -r requirements.txt

# Setup Google Cloud
gcloud auth login
gcloud config set project YOUR_PROJECT_ID

# Environment variables
cp .env.template .env
# Edit .env with Binance API keys + GCP secrets

# Run backtest
python backtest.py --symbol BTCUSDT --days 30

# Start live trading
gunicorn app:app --workers 4
```



## 📊 Key Components
|Module |	Purpose|
|--------|--------|
|trading/	| Strategy logic + TA indicators |
| binance/ |	Real-time API + WebSocket |
| cloud/	| BigQuery logging + Data Studio prep |
| telegram/	| Notifications + monitoring |
| backtest/	| Historical strategy testing |


## 🚨 Production Features
- BigQuery Analytics - Complete trade history

- Data Studio Dashboards - Performance visualization

- Error Recovery - Telegram alerts on failures

- Rate Limiting - Binance API compliance

- Queue Processing - Google Cloud Tasks

- Secret Management - GCP Secret Manager

## 📈 Sample Strategies Tested

- RSI + MACD crossovers
- Bollinger Bands breakouts  
- Volume-weighted momentum
- Multi-timeframe analysis
Backtested + Live traded → BigQuery → Data Studio (2021)

**Built with ❤️ in 2021 - Full trading pipeline**

⭐ Star for more crypto trading projects
