# 📊 Vendor Performance Analytics

An **end-to-end data analytics project** designed to evaluate **vendor performance** using a complete pipeline of **SQL, Python, Power BI (with DAX), and business reporting**.  
This project mirrors **industry standards** for data analysis — from raw data ingestion to actionable insights — covering **logging, data engineering, hypothesis testing, EDA, visualization, and reporting**.

---

## 🚀 Project Overview

Vendors play a critical role in retail and distribution. Measuring their efficiency requires analyzing:
- Sales contribution
- Purchasing efficiency
- Profit margins
- Inventory turnover
- Bulk purchase cost savings

This project answers these questions by building a **robust vendor analytics pipeline**.

---

## ⚙️ Tech Stack

- **SQL (SQLite + dbt)** → Data ingestion, cleaning, dimensional modeling  
- **Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn, SQLAlchemy)** → EDA, hypothesis testing, vendor KPIs  
- **Power BI (DAX)** → Interactive dashboards for vendor contribution, profit margins, and turnover  
- **Reporting** → Automated business-ready reports with statistical validation  


---

## 📈 Key Analyses & Insights

1. **Top Vendor Contribution**
   - Top 10 vendors contribute **65.69% of purchases**, raising **supply chain dependency risks**.

2. **Bulk Purchase Savings**
   - Buying in bulk reduces **unit costs by ~72%** ($10.78 vs. $39.05 small orders).  
   - Encourages vendors to place **larger, more profitable orders**.

3. **Inventory Turnover**
   - $2.71M tied up in unsold inventory.  
   - Identified **low-turnover vendors**, suggesting **stock optimization + clearance strategies**.

4. **Profit Margin Comparison**
   - **Top vendors**: Avg. margin ~31.2%  
   - **Low vendors**: Avg. margin ~41.6%  
   - Indicates **pricing inefficiencies** among low-volume vendors.

5. **Statistical Validation**
   - **t-test** confirms profit margin differences between top & low vendors are **statistically significant**.  
   - Implication: High-margin vendors need **pricing optimization**, while top-sellers should focus on **cost efficiency**.

---

## 🖥 Power BI Dashboard (DAX-Powered)

The **Power BI dashboard** provides:
- Vendor contribution overview  
- Profitability & margin distribution  
- Stock turnover trends  
- Drill-down by brand/vendor  
- DAX measures for **custom KPIs** (e.g., Profit Margin %, Stock Turnover, Sales-to-Purchase Ratio)  

<img width="907" height="592" alt="image" src="https://github.com/user-attachments/assets/21418c66-bc6f-45af-9dd3-c157165f59bd" />

---

## ✅ Final Recommendations

- **Diversify vendor base** to mitigate supply chain risks  
- **Leverage bulk purchasing** for cost savings & efficiency  
- **Optimize slow-moving inventory** with revised order sizes & clearance strategies  
- **Re-evaluate pricing** for high-margin, low-volume brands to boost sales  
- **Enhance marketing & distribution** for underperforming vendors  

---

## 📊 Results

By following this framework, the project demonstrates how **data-driven vendor management** can:  
✔ Improve profitability  
✔ Reduce operational risks  
✔ Enhance purchasing strategies  
✔ Drive sustainable growth  

---

## 🔧 Getting Started

1. Clone the Repository

git clone https://github.com/vickythatguy/vendor-performance-analytics.git
cd vendor-performance-analytics

2. Install Dependencies
pip install -r requirements.txt

3. Ingest Data
python scripts/ingest_data.py
python scripts/get_vendor_summary.py

4. Run Analysis
jupyter lab
# or
jupyter notebook


Open Vendor Performance Analysis.ipynb to run full analysis.

5. Explore Power BI

Open powerbi/vendor_performance.pbix to view interactive dashboards.

👤 Author

Vignesh Subramaniam
🔗 LinkedIn

📂 Portfolio
