# Triangular Arbitrage Bot

A Python-based arbitrage bot that scans multiple cryptocurrency exchanges for triangular arbitrage opportunities using the CCXT library.

## Overview

This bot automatically detects and executes triangular arbitrage trades across exchanges like Binance, Kucoin, Okex, and Huobi. It searches for profitable cycles starting with USDT as the quote currency and considers fees, tick sizes, and order book impact.

## Features

- Multi-exchange arbitrage detection
- Automated trade execution
- Fee and slippage consideration
- Real-time market monitoring
- Telegram notifications for profitable trades
- Comprehensive logging system

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
