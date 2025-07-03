# XTriBot – (Cross-Exchange Triangular Bot)

XTriBot is a Python-based automated trading bot that scans multiple cryptocurrency exchanges for triangular arbitrage opportunities using the CCXT library.

It detects profitable trading cycles starting and ending in USDT, taking into account fees, tick sizes, and order book depth. Designed for real-time execution, XTriBot can also notify you via Telegram and keeps detailed logs of its operations.

---

## Overview

This bot automatically detects and executes triangular arbitrage trades across exchanges like Binance, Kucoin, Okex, and Huobi. It searches for profitable cycles starting with USDT as the quote currency and considers fees, tick sizes, and order book impact.

XTriBot continuously monitors exchanges such as Binance, KuCoin, OKX, and Huobi to:

- [x] Identify arbitrage loops (e.g., USDT → BTC → ETH → USDT)

- [x] Calculate potential profits after accounting for fees, slippage, and market constraints

- [x] Execute trades automatically when thresholds are met

- [x] Send real-time alerts via Telegram




## ✅ Features

- ⚡ **Multi-Exchange Arbitrage Detection**  
   Scans and compares markets across multiple crypto exchanges  

- 🔁 **Automated Trade Execution**  
  Places orders sequentially for profitable arbitrage cycles

- 💸 **Fee & Slippage Awareness**  
  Considers trading fees, order book depth, and price rounding

- 📈 **Real-Time Market Monitoring**  
  Uses live order book data from each configured exchange

- 📩 **Telegram Notifications**  
  Get alerts for profitable trades and system status

- 📝 **Comprehensive Logging**  
  Records all trade activity and diagnostics to a local log file



---

## Prerequisites

- Python 3.7 or higher
- CCXT library
- python-dotenv
- pandas
- numpy
- python-telegram-bot

## Installation

1. Clone the repository
2. Install dependencies: `pip install -r requirements.txt`
3. Copy `config.env.example` to `config.env`
4. Configure your API keys and settings in `config.env`

## Usage

Run the bot:
```bash
python tri_arb_bot.py
```

The bot will:
- Scan for arbitrage opportunities across configured exchanges
- Execute trades when profitable opportunities are found
- Send Telegram notifications for successful trades
- Log all activities to `arbitrage.log`

## Configuration

- Set minimum profit thresholds
- Configure exchange-specific fees
- Adjust message intervals
- Set initial trading amounts
