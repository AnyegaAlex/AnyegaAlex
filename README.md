# Hi, I'm Alex Anyega

**Quantitative Systems Engineer | Full-Stack Architect | Algorithmic Trader**

I build production systems where statistical edge meets code excellence.  
5+ years of experience in low-latency trading infrastructure, MLOps, and distributed systems.

---

## Core Production Systems

### TIES — Trading Infrastructure & Execution System
*Tickflow Capital's proprietary in-house platform for systematic trading.*

- **Engineered** an event-driven backtesting engine processing 7 years of 1-minute tick data, achieving a **75% walk-forward pass rate** (4 out-of-sample windows, 2018–2025) with a Sharpe ratio of **2.10** and avg profit factor of **1.90** across 124 trades.
- **Architected** a 7-layer risk validation gate (kill-switch, drawdown limits, slippage monitoring, preflight validation), enforcing hard daily budget limits and reducing anomalous execution risk to **0%** in live paper-trading.
- **Integrated** MetaTrader 5 for sub-second order dispatch with exponential backoff retry logic and fill reconciliation.
- **Deployed** a full observability mesh using **Prometheus/Grafana/Loki** (12 metrics, 9 alert rules) paired with an immutable, append-only PostgreSQL audit system enabling full trade-decision replay via `trace_id` correlation.
- **Containerized** with Docker and orchestrated on AWS, enabling horizontal scaling for Monte Carlo ensembles of **10,000+ iterations**.

 **Validation Highlights:**
- Best Window Return: **+13.14%** (Window 1, 2020)
- Monte Carlo Confidence: **98.6th percentile**

---

###  Tickflow Intelligence — AI Stock Intelligence Platform
*Open-source (MIT) production platform for stock direction prediction.*

- **Developed** a hybrid forecasting model (50% LSTM / 30% FinBERT sentiment / 20% technicals) serving 10 symbols with 15+ years of historical data.
- **Designed** a REST API gateway with 30+ endpoints (OpenAPI/Swagger) using dual-layer authentication (JWT + PBKDF2-hashed keys) and tiered rate-limiting.
- **Orchestrated** async ETL pipelines (Celery + Redis) for multi-source news ingestion, applying SHA-256 deduplication to reduce redundant processing by an estimated **40%**.
- **Maintained** >99% service availability for automated 7-day prediction tracking via Sentry + UptimeRobot.

 **[Live Demo](https://sentiment-driven-stock-price-predic.vercel.app/)** • **[API Docs](https://sentiment-driven-stock-price-prediction.onrender.com/api/docs/)** • **[Repo](https://github.com/AnyegaAlex/Sentiment-Driven-Stock-Price-Prediction-Using-News-Headlines)**

---

##  Technical Arsenal

| Domain | Technologies |
| :--- | :--- |
| **Quant & ML** | Python, PyTorch, scikit-learn, Pandas, NumPy, FinBERT, MetaTrader5 |
| **Backend** | Django, FastAPI, Celery, Redis, PostgreSQL, WebSockets |
| **Frontend** | React, Chart.js, TailwindCSS |
| **Infra & DevOps** | Docker, AWS (EC2/RDS), Cloudflare, GitHub Actions, Nginx |
| **Observability** | Prometheus, Grafana, Loki, Sentry |

---

##  Connect with Me

I enjoy deep dives into walk-forward validation, risk architecture, async Python, and open-source tooling.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/anyega-alex-kamau)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:anyega.alex.kamau@gmail.com)
[![Calendly](https://img.shields.io/badge/Schedule_30min-00A4EF?style=for-the-badge&logo=calendly&logoColor=white)](https://calendly.com/anyega-alex/30min)

---

## Support My Work

If you find my open-source projects useful, you can support ongoing development:

<p align="center">
  <img width="160" height="160" alt="BNB20QR" src="https://github.com/user-attachments/assets/ffbb43dc-4610-466f-9d4b-56427ca391c0" />
  <img width="160" height="160" alt="TRONQR" src="https://github.com/user-attachments/assets/833f0bfe-ad8e-450b-8345-f3904879180e" />
  <img width="160" height="160" alt="BTCQR" src="https://github.com/user-attachments/assets/e46dc59c-cb87-4944-bb4a-4733a1626d57" />
</p>

<p align="center">
  <sub>BNB Chain (BEP20) &nbsp;·&nbsp; TRON (TRC20) &nbsp;·&nbsp; Bitcoin</sub>
</p>

**USDT / USDC (Recommended)**  
Network: BNB Smart Chain (BEP20)  
`0xCfB8a1b4Abaec2DEF899F7df6F522D705DE58401`

**USDT (Alternative)**  
Network: TRON (TRC20)  
`TVi1M9Kpiaz48eytVzeqJjBd4MBTCbB2TL`

**Bitcoin (BTC)**  
`bc1qd47q5xmc6edlcspn9f3ecakkfaedwrt932w476`

⚠️ *Please only use the networks listed above. Sending on the wrong network will result in permanent loss of funds.*

---
*Building systems that don't lie.*
