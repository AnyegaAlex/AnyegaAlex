# Alex Anyega

## Quantitative Systems Engineer | Full-Stack Architect | Algorithmic Trader

I build production systems where statistical edge meets code excellence.

I am a software engineer with 5+ years of full-stack, AI, and quant development experience. My work spans two production systems:

- Tickflow Intelligence: Open-source AI stock platform with LSTM + FinBERT, 30+ API endpoints, and 68-page documentation
- TIES: Trading Infrastructure and Execution System with 7-gate risk controls, MT5 integration, and 75 percent walk-forward pass rate

---

## Featured Projects

### Tickflow Intelligence - AI Stock Intelligence Platform

Production AI platform for stock direction prediction using LSTM + FinBERT sentiment analysis.

An open-source (MIT) platform combining:

- Hybrid Model: 50 percent LSTM + 30 percent FinBERT sentiment + 20 percent technical indicators
- 30+ REST API endpoints with OpenAPI and Swagger documentation
- Multi-source news ingestion from Alpha Vantage, Finnhub, and Yahoo Finance with SHA-256 deduplication
- React dashboard with real-time visualisations and prediction tracking
- Dual-layer authentication: JWT and PBKDF2-hashed API keys with tiered rate limiting
- Async pipelines: Celery and Redis for news processing
- Observability: Sentry, UptimeRobot, and structured JSON logging
- Automated resolution: 7-day prediction tracking via cron jobs

Supports multiple symbols with 15+ years of historical data.

| Component | URL |
|-----------|-----|
| Live Demo | https://sentiment-driven-stock-price-predic.vercel.app/ |
| Swagger API Docs | https://sentiment-driven-stock-price-prediction.onrender.com/api/docs/ |
| GitHub | https://github.com/AnyegaAlex/Sentiment-Driven-Stock-Price-Prediction-Using-News-Headlines |

Tech Stack: React, Django, PyTorch, FinBERT, PostgreSQL, Redis, Celery, Docker, Vercel, Render

---

### TIES - Trading Infrastructure and Execution System

Production trading engine for research, validation, and live execution. Built by traders, for traders.

TIES is Tickflow Capital's proprietary in-house platform for systematic trading strategy development and deployment.

#### Research Platform

| Component | Description |
|-----------|-------------|
| Backtesting Engine | Event-driven backtesting processing 7 years of tick data at 1-minute resolution |
| Monte Carlo Simulation | 10,000 iteration ensemble for robustness testing |
| Walk-Forward Validation | 4 independent test windows with 24-month training and 12-month testing |
| Statistical Analysis | t-statistic, p-value calculation, confidence intervals |
| Regime Detection | Hidden Markov Models for market regime classification |

Key Metric: 75 percent pass rate across 4 out-of-sample windows (2018 to 2025)

#### Risk Engine - 7 Layer Validation

| Gate | Control |
|------|---------|
| 1 | Kill Switch with 3-level emergency stop (pause, halt, kill) |
| 2 | Daily Budget Gates with hard limits on daily trading exposure |
| 3 | Drawdown Controls with maximum drawdown limits enforced |
| 4 | Position Constraints with caps on position sizes |
| 5 | Calendar-Based Restrictions with time-based trading rules |
| 6 | Slippage Monitoring for broker anomaly detection |
| 7 | Preflight Validation with pre-trade checks before any order dispatch |

#### Execution Infrastructure

| Component | Description |
|-----------|-------------|
| Low-Latency Execution | Sub-second order dispatch through MT5 |
| Retry Logic | Automatic retry with exponential backoff |
| Fill Reconciliation | Order-to-fill matching and verification |
| Slippage Modeling | Realistic market condition simulation |

#### Observability Stack

| Tool | Purpose |
|------|---------|
| Prometheus | 12 production metrics monitored |
| Grafana | Real-time dashboards |
| Loki | Centralised log aggregation |
| Alertmanager | 9 alert rules for system anomalies |
| Sentry | Real-time error capture |

#### Audit System

- Append-Only PostgreSQL Log: Every decision has a trace_id
- Full Replay Capability: Any decision chain can be replayed
- No Application-Level Deletes: Immutable record of all actions
- Trace ID Correlation: Decision to execution to outcome tracking

#### Performance Metrics From Validation Data

| Metric | Value |
|--------|-------|
| Pass Rate | 75 percent (3 of 4 windows) |
| Avg Profit Factor | 1.90 (passing windows: 2.27 average) |
| Total Trades | 124 across 4 windows |
| Best Window Return | +13.14 percent (Window 1, 2020) |
| Sharpe Ratio | 2.10 |
| Monte Carlo Confidence | 98.6th percentile |

Tech Stack: Python, FastAPI, MT5, PostgreSQL, Redis, Prometheus, Grafana, Loki, Docker, AWS, Cloudflare

Website: https://tickflowcapital.com

---

## Tech Stack

### Backend and APIs

Python, Django, FastAPI, PostgreSQL, Redis

### Quant and Trading

MetaTrader5, Pandas, NumPy, scikit-learn, PyTorch

### Frontend

React, Chart.js, TailwindCSS

### Infrastructure and DevOps

Docker, AWS, Cloudflare, GitHub Actions

### Observability

Prometheus, Grafana, Loki, Sentry

---

## Certifications

- Google Analytics Certification - Skillshop - Aug 2023
- Google Analytics Individual Qualification - Google - Aug 2023
- IAB Digital Marketing Foundations - Google Digital Garage - Aug 2022
- Learn Elementor and WordPress - Udemy - Feb 2023

---

## Let's Connect

I enjoy conversations about:

- Quant and Trading: Walk-forward validation, risk architecture, MT5 integration, regime classification
- Full-Stack Systems: API design, async Python, observability, audit logging, rate limiting
- Open Source: Developer tools, documentation, community building

LinkedIn: https://linkedin.com/in/anyega-alex-kamau
Gmail: anyega.alex.kamau@gmail.com
GitHub: https://github.com/AnyegaAlex
Calendly: https://calendly.com/anyega-alex/30min

---

Building systems that don't lie.
