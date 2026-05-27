# ⚡️ ForgeX

> High-performance, low-latency Forex backtesting and market simulation.

Welcome to the **ForgeX** GitHub Organization. We are building a streamlined, accessible SaaS platform designed to give day traders and prop-firm candidates a zero-latency environment to practice trade execution, backtest strategies, and analyze session performance.

Our core development philosophy is simple: **Learn, build, ship, repeat.** We prioritize lean architecture, rapid prototyping, and bypassing expensive third-party APIs by managing raw, high-density MT5 tick data locally.

---

## 🏗️ Core Architecture

ForgeX is built on a decoupled architecture to ensure the simulation engine remains fast and the UI remains highly responsive when parsing millions of rows of 1M (one-minute) historical OHLCV data.

* **Data Ingestion:** Automated Python scripts to extract, parse, and structure minute-by-minute MT5 historical data.
* **Simulation Engine:** A lightweight, highly parallelized FastAPI backend serving historical chunks with sub-second latency.
* **Terminal UI:** A dark-mode, canvas-based React frontend utilizing TradingView Advanced Charts for real-time order execution, dynamic risk calculation, and visual P&L tracking.

---

## 📦 Repositories

The ForgeX ecosystem is divided into the following core private repositories:

| Repository | Description | Status |
| :--- | :--- | :--- |
| 🗄️ **`forgex-engine`** | The Python/FastAPI backend API and SQLite/PostgreSQL database schema. Handles historical data serving, user state, and analytic calculations. | *Active* |
| 🖥️ **`forgex-terminal`** | The Vite/React frontend application. Houses the TradingView implementation, drag-and-drop order UI, and metrics dashboard. | *Active* |
| 📊 **`forgex-data-pipeline`** | Python scripts for extracting MT5 CSVs, normalizing data formats, and batch-inserting millions of rows into the database. | *Active* |

---

## 🛠️ Tech Stack

### Frontend
* **Framework:** React (Vite)
* **Charting:** TradingView Lightweight / Advanced Charts (HTML5 Canvas)
* **Styling:** CSS Variables / Tailwind CSS (Dark Terminal UI)

### Backend & Data
* **Server:** Python / FastAPI
* **Database (Local MVP):** SQLite
* **Database (Production):** PostgreSQL
* **Infrastructure:** Render / Railway

### Auth & Payments (Upcoming)
* **Authentication:** Supabase (JWT)
* **Billing:** Stripe Subscriptions

---

## 👥 Team

ForgeX is maintained by:
* **Prajwal**
* **Advay**

*Focused on engineering systems with zero fluff.*
