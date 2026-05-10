# Smart Momentum Ticker Scanner — Android APK (EU & USA Markets)

<img width="996" height="2048" alt="image" src="https://github.com/user-attachments/assets/f63cdbac-b23f-4803-8be3-f522d5183d25" />

Android application that scans **European and US equities** and returns **high-probability momentum candidates** using institutional-grade quantitative filters inspired by **trend following**, **volatility regime analysis**.

WARNING: Portfolio / research project. Educational use only. No financial advice.

---
📦 **APK Download**  
➡️ Available in the [Releases](../../releases) section of this repository.

---

## What this app does (in one sentence)

It transforms raw market data into **actionable momentum candidates** using **regime filtering + volatility contraction + accumulation detection**, delivered as a **mobile-first scanner**.

---

## Markets covered

- 🇪🇺 **Europe** (LSE, Euronext, Xetra, etc.)
- 🇺🇸 **United States** (NYSE / NASDAQ)

## Output: actionable stock candidates

The app classifies stocks into **four distinct momentum regimes**, each designed for a different trading intention:

### 1. Smart Momentum (core strategy)
High-quality trend continuation candidates.

Designed for:
- Swing trading
- Position trading
- Trend participation with reduced noise

### 2. Missile
Explosive breakouts driven by **abnormal volume + price expansion**.

Designed for:
- Momentum bursts
- News / flow-driven moves
- Short holding periods

### 3. Early Momentum
Pre-breakout setups detected via **volatility contraction and volume drought**.

Designed for:
- Anticipatory positioning
- Volatility expansion strategies

### 4. Stable Trend
Clean, mature trends with **low volatility expansion risk**.

Designed for:
- Capital preservation within trends
- Low-noise environments

---

## Quantitative foundations

This scanner is **not indicator stacking**.  
It is built on **market microstructure–aware principles**:

### 1. Regime filtering

- Trades are only considered when the market is in a **favorable regime**
- Uses **ADX trend strength** and **directional persistence**
- Avoids applying momentum in mean-reverting conditions

> Key idea: *no signal is valid outside the right regime*

---

### 2. Volatility contraction → expansion logic

- Detects **ATR compression over multi-window horizons**
- Requires a **confirmed volatility uptick**
- Filters out false breakouts during volatility decay

This follows the same logic behind:
- Volatility breakout systems
- Event-based sampling (price only matters when something changes)

---

### 3. Accumulation & participation 

- OBV slope and breakout detection
- Asymmetric volume analysis:
  - volume on up-bars vs down-bars
- Rejects price moves unsupported by participation

> No volume → no trade

---

### 4. Momentum confirmation 

- RSI used **only after regime and volatility validation**
- Momentum must be:
  - directional
  - persistent
  - accelerating

RSI is never used as a standalone signal.

---

## Why this is different from retail scanners

| Typical Retail Scanner | This App |
|-----------------------|---------|
| Fixed RSI thresholds | Regime-conditional momentum |
| Time-based bars | Event-driven logic |
| Indicator stacking | Orthogonal filters |
| No volatility logic | Explicit volatility regime |
| No volume asymmetry | Participation validated |
| Desktop only | Mobile-first execution |

---

## User workflow

1. Select **EU or USA market**
2. Run scan
3. Review candidates by strategy
4. Focus analysis only on **pre-filtered, regime-valid stocks**
5. Apply personal execution rules (broker, timeframe, sizing)

The app **does not place trades** — it delivers **signal quality**, not execution.

---

## Architecture (high level)

- **Android (Java)**
- Modular quantitative engine:
  - Indicators
  - Strategy classifiers
  - Regime filters
- Stateless scanning (no curve fitting on device)
- CSV export / visual inspection friendly

---

## Intended audience

- Quantitative traders
- Systematic swing traders
- Data scientists interested in financial signal engineering
- Fintech / trading infrastructure roles

---

## What this project demonstrates

- Translation of **quant research concepts into production code**
- Separation of **signal generation vs execution**
- Understanding of **market regimes, volatility, and participation**
- Ability to package research into **usable software**

---

## Limitations

- Uses public market data (no L2 / no proprietary feeds)
- No intraday microstructure modeling
- No execution or portfolio optimization
- No curve-fitted backtest marketing

This is a **signal-quality engine**, not a promise machine.

---

📦 **APK Download**  
➡️ Available in the [Releases](../../releases) section of this repository.


## Disclaimer

This application is for research and educational purposes only.  
It does not constitute financial advice.

---

## License

Add an explicit open-source license (MIT / Apache-2.0 recommended).
