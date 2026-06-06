# Alex Anyega

## Quantitative Systems Engineer | Full-Stack Architect | Algorithmic Trader

**I build production systems where statistical edge meets code excellence because markets don't forgive wishful thinking, and neither do I.**

I'm a software engineer with 5+ years of full-stack, AI, and data engineering experience, and a quantitative trader who validates every strategy with walk-forward analysis, Monte Carlo confidence, and live capital. The result is systems that are not only beautifully engineered but also statistically trustworthy, whether they're trading XAUUSD or powering a budgeting app used by 60%+ of beta testers.

---

## The Intersection: Why Development + Financial Markets?

Two sides of the same coin drive everything I build.

### 1. The Trader's Side (The Heart)

I'm a trader first. Not a theorist. A practitioner.

I grew a live account from $20 to over $10,000. Not through luck, but through discipline, risk management, and understanding market microstructure. Every gain taught me humility. Every loss taught me respect for the craft.

Trading isn't just charts and candlesticks. It's risk psychology, watching drawdown test your soul at 3 AM. It's execution precision, one fat-finger click away from disaster. It's regime awareness, knowing when not to trade is the ultimate edge.

I've felt the sting of a losing streak. I've felt the rush of a perfectly executed reversal. That lived experience, not theory, informs every line of code I write.

### 2. The Engineer's Side (The Hands)

I went to school for this. Bachelor of Science in Computer Science (Second Class Upper Division) from Maasai Mara University.

That formal foundation gave me data structures and algorithms, so efficient systems don't happen by accident. Database management for append-only audit logs, ACID compliance, and time-series at scale. Machine learning for feature engineering that actually generalizes. Web development for full-stack SaaS products, not just trading bots.

But theory without practice is useless. So I built.

### When They Meet: TIES

TIES (Trading Intelligence & Execution System) is the fusion.

| Trader's Input | Engineer's Implementation |
|----------------|---------------------------|
| "I need a kill switch when drawdown hits 8%" | 7-gate risk engine with Redis-backed halt states |
| "Why did that trade enter?" | Append-only audit log, every decision replayed by trace_id |
| "My broker's spreads exploded at news" | Slippage monitoring and anomaly flagging |
| "Backtesting looked great, live trading failed" | Walk-forward validation, 75% pass rate across 7 years |
| "I can't watch charts 24/5" | Event-driven async architecture with Telegram C&C |

The result is a production trading system that trades real capital through MT5, built by a trader who codes, not a coder who trades.

### But It's Not Just Trading

The same obsessive attention to data integrity, real-time processing, and user value lives in my full-stack SaaS projects.

Trading taught me risk management. CS school taught me systems thinking. Together, they make me dangerous in a good way.

**The bottom line:** I'm not an academic. I'm not a backtest overfitter. I'm a trader who can build the infrastructure I need and then sell the excess tools to others who share the same pain.

-> [See what I've built](https://tickflowcapital.com)

---

## Featured Project: TIES (Trading Intelligence & Execution System)

**The production trading engine powering Tickflow Capital's research and validation products.**

TIES is our internal, Python-first algorithmic trading system, battle-tested on live capital and now partially commercialized through Tickflow Capital. It's not a hobby bot. It's the infrastructure we trust with real money.

**Tech Stack:** Python/FastAPI, PostgreSQL, Redis, MT5 API, Prometheus, Grafana, Loki, Docker, Cloudflare

### What TIES Does

| Layer | Capability |
|-------|-------------|
| Signal Engine | Multi-factor scenario detection with regime-aware scoring |
| Risk Engine | 7 cascading gates: kill switch, budget, drawdown, position caps, anomaly detection |
| Execution Bridge | Preflight validation, MT5 dispatch, fill reconciliation, position tracking |
| Observability | Prometheus + Grafana + Loki + Alertmanager + Sentry |
| Audit System | Append-only PostgreSQL log with full trace replay |

### Validated Through Live Capital

TIES has been validated using walk-forward methodology on 7+ years of XAUUSD data, the same rigorous process we offer to clients. Every statistical claim is backed by independent out-of-sample periods and Monte Carlo analysis.

**The methodology is public. The specific strategy parameters are not.**

-> [View complete walk-forward validation results](https://tickflowcapital.com)

### Commercial Products Built on TIES

Tickflow Capital offers three products extracted directly from our internal TIES deployment.

| Product | For | Price |
|---------|-----|-------|
| Strategy Validation | Prop firms and systematic traders needing statistical edge assessment | $3,500 one-time |
| Market Context API | Real-time regime classification, volatility state, structural levels | $1,500/month |
| Enterprise Risk Suite | White-label risk gate infrastructure with full audit trail | Custom quote |

-> [See product details and sample reports](https://tickflowcapital.com)

### Why This Matters

We don't sell what we wouldn't use ourselves. Every TIES component, every risk gate, every audit log, every observability metric was built because we needed it to trade our own capital safely.

The software is the product. The live trades are the proof.

**Website:** [tickflowcapital.com](https://tickflowcapital.com)
**Research:** Walk-forward validation, VPS OpSec, Backtesting paradox
**Contact:** info@tickflowcapital.com

**Repos:** [GitHub](https://github.com/AnyegaAlex/) for open-source projects unrelated to TIES core IP.

---

## Quant Philosophy: Why Rigor Is Non-Negotiable

**The problem:** Most retail traders backtest to confirm their bias.
**The solution:** Walk-forward validation with independent out-of-sample testing.

We don't trade what we can't validate. Every strategy deployed through TIES must pass a three-stage gauntlet before seeing live capital.

### Validation Hierarchy

| Stage | What It Does | Why It Matters |
|-------|--------------|----------------|
| In-Sample | Train on historical data | Proof of concept |
| Out-of-Sample (Walk-Forward) | Test on held-out periods | Generalization test, catches curve-fitting |
| Blind Hold-Out | Evaluate on unseen future data after live trading starts | Ultimate truth |

**Rule:** If all three agree, you have an edge. If they diverge, you're curve-fit.

-> [View complete walk-forward methodology](https://tickflowcapital.com)

### Metrics That Define an Edge

| Metric | Threshold | Why |
|--------|-----------|-----|
| Profit Factor | > 1.5 (excellent > 1.9) | Gross profit divided by gross loss, simple and unforgiving |
| Sharpe Ratio | > 0.5 | Risk-adjusted return |
| Max Drawdown | Hard cap at 8% | System halts if exceeded, non-negotiable |
| Win Rate | Secondary | Risk/reward ratio matters more than hit rate |
| Monte Carlo Confidence | > 98% of shuffled sequences beat breakeven | Separates edge from luck |

### Intermarket Context (XAUUSD Focus)

Gold in isolation is noise. Gold relative to macro is signal.

| Signal | Role |
|--------|------|
| DXY (Dollar Index) | Inverse correlation, primary filter |
| VIX (Volatility Index) | Regime classification (LOW/NORMAL/ELEVATED/EXTREME) |
| US10Y (Bond Yields) | Real rate direction, opportunity cost signal |
| Economic Calendar | No entry 30 minutes before or after high-impact events |

Macro bias classification (bullish/bearish/neutral) weights every signal before it reaches the risk engine.

### What Walk-Forward Validation Looks Like

Training Period (24 months) -> Test Period (12 months) -> Result

2018-2019 -> 2020 -> PASS
2019-2020 -> 2021 -> FAIL
2020-2021 -> 2022 -> PASS
2021-2022 -> 2023 -> PASS
2022-2023 -> 2024 -> PASS
2023-2024 -> 2025 -> PASS

**Our 7-year XAUUSD validation:** 75% pass rate across independent windows.

-> [See detailed results](https://tickflowcapital.com)

### The Backtest Paradox

90% of strategies fail in live trading. Not because the idea was bad, but because the validation was lazy.

**Common pitfalls we avoid:**

| Pitfall | Our Fix |
|---------|---------|
| Lookahead bias | Signals use only historically available data |
| Survivorship bias | Include delisted instruments in testing |
| Slippage ignorance | 3.0 pip spread assumption plus execution quality audits |
| Regime overfitting | Test across bull, bear, and sideways markets |
| Transaction cost neglect | Realistic commission and swap modeling |

-> [Read full article: The Backtest Paradox](https://tickflowcapital.com)

### Why This Philosophy Is Built Into TIES

Every risk gate, every audit log, every observability metric exists because statistical rigor isn't optional. It's the moat between profitable systems and expensive lessons.

| Component | Enforces |
|-----------|----------|
| 7-gate Risk Engine | Drawdown, budget, and position discipline |
| Append-Only Audit Log | Full replayability, no hiding decisions |
| Prometheus + Grafana | Real-time equity curves and risk state |
| Slippage Monitoring | Broker anomaly detection (spread explosion, time desync) |

**We don't sell what we wouldn't use ourselves.** TIES runs our own capital. Every product Tickflow Capital offers was extracted from a system that already proved itself in live markets.

**Website:** [tickflowcapital.com](https://tickflowcapital.com)
**Research:** Walk-forward validation, VPS OpSec, Backtesting paradox
**Contact:** info@tickflowcapital.com

---

## Other Notable Engineering Projects

### Budget Buddy - AI-Driven Personal Finance Platform

React + Firebase responsive budgeting app with custom expense categories. ML-powered recommendations for spending predictions and goal tracking. Achieved 60% user engagement during beta testing.

[Live demo](https://budget-buddy-rose-phi.vercel.app/) | [GitHub](https://github.com/AnyegaAlex/budget-buddy)

### Machine Learning Stock Prediction Platform

DistilBERT sentiment analysis at 92% accuracy combined with HistGradientBoostingClassifier at 82% test accuracy. Features SHAP explainability, batch CSV predictions, and an interactive Gradio UI.

[Hugging Face Space](https://huggingface.co/spaces/AnyegaAlex/stock-prediction-analytics)

### Global Cost-of-Living Explorer

Django REST API with React frontend and Leaflet maps to compare inflation, wages, and currency trends across 50+ countries. Redis caching reduced query time by 50%.

[GitHub](https://github.com/AnyegaAlex/Cost-of-Living-Explorer)

### Sentiment-Driven Stock Price Prediction (Real-Time)

FinBERT sentiment analysis with Celery/Redis async pipeline, integrating Alpha Vantage and Yahoo Finance. Features SHA-256 deduplication and Dockerised deployment.

[Live demo](https://sentiment-driven-stock-price-predic.vercel.app)

---

## Tech Stack

### Backend & Data Infrastructure

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DD0031?style=flat-square&logo=redis&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-8B4513?style=flat-square)

### Quant & Market Data

![MetaTrader5](https://img.shields.io/badge/MetaTrader5-008B8B?style=flat-square)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)

### Frontend & Visualization

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![D3.js](https://img.shields.io/badge/D3.js-F9A03C?style=flat-square&logo=d3.js&logoColor=white)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=flat-square&logo=chart.js&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

### Observability & DevOps

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F2CC0C?style=flat-square&logo=grafana&logoColor=black)
![Loki](https://img.shields.io/badge/Loki-8B4513?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

---

## GitHub Analytics

<div align="center">
  
  ![GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=AnyegaAlex&theme=radical&hide_border=true)
  
</div>

---

## Certifications

![Google Analytics](https://img.shields.io/badge/Google_Analytics-Certified-4285F4?style=flat-square&logo=google-analytics&logoColor=white)
![IAB Digital Marketing](https://img.shields.io/badge/IAB_Digital_Marketing-Certified-FF6F00?style=flat-square)

---

## Let's Connect

I enjoy conversations about:

- Quant and trading: backtesting methodology, walk-forward validation, risk architecture, MT5 integration, regime classification
- Full-stack systems: FastAPI, async Python, observability, audit logging, rate limiting
- Commercial validation: product-market fit for developer tools, SaaS pricing, founder-led sales

<div align="center">
  
  [![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/anyega-alex-kamau)
  [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anyega.alex.kamau@gmail.com?subject=Trading%20Systems%20%7C%20Quant%20Chat)
  [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AnyegaAlex)
  [![Calendly](https://img.shields.io/badge/Schedule_30min-00A4EF?style=for-the-badge&logo=calendly&logoColor=white)](https://calendly.com/anyega-alex/30min)
  
</div>

<div align="center">
  
  ![Visitor Count](https://komarev.com/ghpvc/?username=AnyegaAlex&color=blueviolet&style=flat-square)
  
  *Building systems that don't lie. Trading capital on them to prove it.*
  
</div>
