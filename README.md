# XTriBot – (Cross-Exchange Triangular Bot)

XTriBot is a Python-based automated trading bot that scans multiple cryptocurrency exchanges for triangular arbitrage opportunities using the CCXT library.

It detects profitable trading cycles starting and ending in USDT, taking into account fees, tick sizes, and order book depth. Designed for real-time execution, XTriBot can also notify you via Telegram and keeps detailed logs of its operations.

---

## 🔍 Overview

This bot automatically detects and executes triangular arbitrage trades across exchanges like Binance, Kucoin, Okex, and Huobi. It searches for profitable cycles starting with USDT as the quote currency and considers fees, tick sizes, and order book impact.

XTriBot continuously monitors exchanges such as Binance, KuCoin, OKX, and Huobi to:

- [x] Identify arbitrage loops (e.g., USDT → BTC → ETH → USDT)

- [x] Calculate potential profits after accounting for fees, slippage, and market constraints

- [x] Execute trades automatically when thresholds are met

- [x] Send real-time alerts via Telegram

---



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

## 🧰 Prerequisites  

**Make sure you have the following installed:**
- Python 3.7 or higher
- CCXT library
- python-dotenv
- pandas
- numpy
- python-telegram-bot

---

## 📦 Installation

1. Clone the repository
    ```bash
    git clone https://github.com/yourusername/XTriBot.git
    cd XTriBot
    ```

2. Install dependencies: `
   ```bash
   pip install -r requirements.txt
   ```
3. Copy `config.env.example` to `config.env`
4. Configure your API keys and settings in `config.env`
 
Open config.env and add your API keys, Telegram credentials, and custom settings.

---

## ▶️ Usage
To run the bot:
```bash
python tri_arb_bot.py
```
Once started,the bot will:
- Scan for arbitrage opportunities across configured exchanges
- Execute trades when profitable opportunities are found
- Send Telegram notifications for successful trades
- Log all activities to `arbitrage.log`


---


## ⚙️ Configuration

Customize behavior in `config.env` :

- Set minimum profit thresholds
- Define exchange-specific trading fees
- Adjust order update/message intervals
- Configure initial trading capital per exchange
- Enable or disable test mode

----

## 📬 Telegram Integration

XTriBot supports Telegram alerts. To enable:

1. Create a Telegram bot via [@BotFather](https://t.me/BotFather)
2. Get your **bot token** and **chat ID**
3. Add them to your `config.env` file

----

## 🛡️ Disclaimer

**This bot is intended for educational and research purposes only. Use at your own risk.**    
**Cryptocurrency trading involves significant financial risk, and you are solely responsible for your trades and API usage.**

---

## 📄  License  

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as per the license terms.

---

## 🤝  Contact & Contributions

We welcome contributions to enhance this project! Whether it's improving the model, adding new features, or fixing bugs, your help is greatly appreciated. 

**To contribute:**

- Fork the repository.

- Create a new branch.

- Submit a pull request with your changes.

---

For inquiries, feedback, or collaboration, feel free to open an issue or reach out via 📧 [**SANCHIT**](mailto:sanchitsharma31@gmail.com).

---

---
