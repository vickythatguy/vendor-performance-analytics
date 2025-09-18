# 📊 Vendor Performance Analytics

_End-to-end analytics project using **SQL, Python, and Power BI** to evaluate vendor contribution, profitability, stock turnover, and purchasing efficiency._

![Made with Python](https://img.shields.io/badge/Python-3.10+-blue)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)
![Power BI](https://img.shields.io/badge/Power%20BI-Report-yellow)

---

## 🚀 Project Overview
- Ingest vendor transactional data and stage it in a local database.
- Perform **EDA** (distributions, correlations, outliers).
- Build **Top Vendors / Brands** analyses and Pareto charts.
- Evaluate **bulk purchasing** impact on unit costs.
- Compute **profitability metrics**: Gross Profit, Profit Margin, Stock Turnover, Sales/Purchase Ratio.
- Run **confidence intervals** and **hypothesis tests** (t-tests) on profit margins.
- Design a **Power BI dashboard** for executive reporting.

---

## 📂 Repository Structure

├── Draft.ipynb # Notebook used up to EDA (early exploration)

├── EDA.ipynb # Supporting exploration/plots

├── Vendor Performance Analysis.ipynb# Main notebook: stats, tests, insights

├── get_vendor_summary.py # Builds vendor_sales_summary from source tables

├── ingestion_db.py # CSV → DB ingestion

├── README.md # This file

└── requirements.txt # Python dependencies



**Dataset:** Stored on Google Drive →  
🔗 https://drive.google.com/drive/folders/1au8URS7ZlzxIVMv2C-tODAJ23DmBxJTT?usp=drive_link

> `Draft.ipynb` is the notebook I used through EDA; after that I continued in `Vendor Performance Analysis.ipynb` for deeper analysis and statistical testing.

---

## 🧠 Key Analyses & Visuals
- Top 10 vendors/brands by sales (labeled horizontal bars with human-readable values, e.g., “7.9M”).
- **Pareto chart**: Vendor contribution to total purchases (bar + cumulative % line).
- **Donut chart**: Top-10 vendor share vs “Other Vendors”.
- **Bulk purchasing**: Unit price vs order size buckets (Small/Medium/Large) with summary insights.
- **Confidence intervals** for profit margins (top vs low performers) and **t-tests** for significance.

---

## 🔧 Tech Stack
- **Python**: pandas, numpy, matplotlib, seaborn, scipy
- **SQL/SQLite** (local dev)
- **Power BI** (dashboard/reporting)

---

## 🏁 Getting Started

### 1) Clone the repo
```bash
git clone https://github.com/<your-username>/vendor-performance-analytics.git
cd vendor-performance-analytics
```
### 2) Create & activate a virtual environment
```bash
# Windows (PowerShell)
python -m venv .venv
.venv\Scripts\Activate.ps1

# macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
```
### 3) Install dependencies
```bash
pip install -r requirements.txt
```
### 4) Get the data

Download the CSVs from Google Drive and place them in a local folder, e.g. ./data/.

# Drive link: https://drive.google.com/drive/folders/1au8URS7ZlzxIVMv2C-tODAJ23DmBxJTT?usp=drive_link

Folder expected by ingestion_db.py: data/ (you can change it in the script if needed).

### 5) Ingest the data into a local DB
```bash
python ingestion_db.py
```
This will create (or update) a local SQLite DB (e.g., inventory.db) and load the CSV tables.

---

### 6) Build the vendor summary table
```bash
python get_vendor_summary.py
```
This script creates a vendor_sales_summary table with consolidated metrics:

GrossProfit

ProfitMargin

StockTurnover

SalesToPurchaseRatio

…and more KPIs.

### 7) Run the notebooks

Start Jupyter and explore the analysis step by step:

Draft.ipynb → Exploratory Data Analysis (EDA phase)

Vendor Performance Analysis.ipynb → Main analysis, statistical tests, and visualization
📈 Power BI (Coming Soon)

The Power BI dashboard (.pbix file + screenshots) will include:

Vendor contribution overview

Profitability & margin distribution

Stock turnover & ordering efficiency

Drill-down by brand/vendor

✅ To-Do / Next Steps

 Upload the Power BI .pbix report

 Add unit tests for the SQL/Python transformations

 Parameterize ingestion paths using .env

 (Optional) Add a Dockerfile for one-shot reproducibility

👤 Author

Vignesh Subramaniam
🔗 LinkedIn

📦 Requirements

To run the notebooks and scripts, install the dependencies:

pandas>=2.0
numpy>=1.24
matplotlib>=3.7
seaborn>=0.13
scipy>=1.11
jupyterlab>=4.0
sqlalchemy>=2.0


👉 You can paste this straight into your README.md.  

Do you also want me to add a **small "Sample Output" section** (with placeholders for charts) so your repo looks more visual when people scroll through it on GitHub?
