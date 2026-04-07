# 🚛 Trucking Operations Analytics

**End-to-end Data Analytics project** on a trucking company's operational database — covering route profitability, driver performance, fleet utilization, fuel efficiency, and safety analysis.

> Built by a logistics professional transitioning into data analytics. Domain knowledge + data skills = business-relevant insights.

---

## 📦 Dataset

**Source:** [Logistics Operations Database – Kaggle](https://www.kaggle.com/datasets/yogape/logistics-operations-database)

14 relational tables | ~85,000 trips | 2022–2023 data

| Table | Rows | Description |
|---|---|---|
| `trips` | 85,411 | Core trip records with fuel, distance, duration |
| `loads` | 85,411 | Shipment details, revenue, customer |
| `delivery_events` | 170,821 | Pickup/delivery timestamps, on-time flags |
| `fuel_purchases` | 196,443 | Fuel transactions by trip and driver |
| `drivers` | 150 | Driver profiles, experience, CDL class |
| `trucks` | 120 | Fleet inventory, make, model year |
| `maintenance_records` | 2,920 | Service history, downtime, costs |
| `safety_incidents` | 170 | Accidents, violations, damage costs |
| `routes` | 58 | Origin–destination lanes, base rates |
| `customers` | 200 | Accounts, contract types, revenue potential |

---

## 🗂️ Data Model (ERD)

![ERD](docs/erd_schema.png)

---

## 🔍 Analysis Modules

### 1. Route Profitability [`sql/01_route_profitability.sql`]
- Revenue per mile by lane (origin → destination)
- Top 10 most and least profitable routes
- Fuel surcharge vs actual fuel cost gap

**Key finding:** *[Fill in after running analysis — e.g. "Atlanta → Chicago generates $2.31/mile vs fleet avg of $1.87"]*

---

### 2. Driver Performance [`sql/02_driver_performance.sql`]
- On-time delivery rate per driver
- MPG ranking — who burns excess fuel?
- Revenue per mile by driver (top vs bottom quartile)

**Key finding:** *[Fill in after running analysis]*

---

### 3. Fleet Utilization [`sql/03_fleet_utilization.sql`]
- Utilization rate per truck (monthly)
- Maintenance downtime vs revenue lost
- Cost per mile by truck age (newer vs older units)

**Key finding:** *[Fill in after running analysis]*

---

### 4. Fuel Efficiency [`sql/04_fuel_efficiency.sql`]
- Average MPG by route and season
- Cheapest refueling locations (avg price per gallon)
- Fuel price trend 2022 vs 2023

**Key finding:** *[Fill in after running analysis]*

---

### 5. Safety Analysis [`sql/05_safety_analysis.sql`]
- Incident rate per 1M miles by driver
- Preventable vs non-preventable breakdown
- Correlation between idle time and incident frequency

**Key finding:** *[Fill in after running analysis]*

---

## 📊 Dashboard

Built in **Power BI Desktop**. See screenshots below.

![Dashboard](dashboard/screenshots/overview.png)

---

## 🛠️ Tools & Stack

| Layer | Tool |
|---|---|
| Data exploration | Python, Pandas, Seaborn |
| SQL analysis | DuckDB (runs directly on CSV files) |
| Visualization | Power BI Desktop |
| Environment | VS Code + Jupyter extension |
| Version control | Git + GitHub |

---

## 📁 Project Structure

```
trucking-operations-analytics/
│
├── README.md
├── data/                          # Not included — download from Kaggle link above
├── sql/
│   ├── 01_route_profitability.sql
│   ├── 02_driver_performance.sql
│   ├── 03_fleet_utilization.sql
│   ├── 04_fuel_efficiency.sql
│   └── 05_safety_analysis.sql
├── notebooks/
│   └── eda_trucking.ipynb
├── dashboard/
│   └── screenshots/
└── docs/
    └── erd_schema.png
```

---

## ▶️ How to Run

```bash
# 1. Clone the repo
git clone https://github.com/YOUR_USERNAME/trucking-operations-analytics.git

# 2. Install dependencies
pip install duckdb pandas matplotlib seaborn jupyter

# 3. Download dataset from Kaggle and place CSVs in /data/

# 4. Open notebook
jupyter notebook notebooks/eda_trucking.ipynb

# 5. Run SQL queries via DuckDB in the notebook or standalone
```

---

## 💼 Skills Demonstrated

`SQL` · `Python` · `Pandas` · `DuckDB` · `Power BI` · `Exploratory Data Analysis` · `Data Modeling` · `Logistics Domain Knowledge`

---

## 👤 About

Built as part of a career transition from **Freight Forwarding (Speditionskaufmann)** to **Data Analytics**. Logistics background means every query has a real operational context behind it.
