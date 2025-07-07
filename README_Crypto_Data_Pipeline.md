
# 🚀 Designing a Scalable Cryptocurrency Data Pipeline Using Azure & Databricks

This project delivers a cloud-native, production-grade ELTL pipeline for real-time cryptocurrency market data, designed for IntelloBank. It leverages Azure Blob Storage, Databricks Auto Loader, Delta Live Tables, and Power BI within a Medallion Architecture to enable automated data ingestion, transformation, and analytics.

---

## ❓ Problem Statement

Traditional methods of collecting and analyzing cryptocurrency data at IntelloBank were manual, fragmented, and not scalable. This resulted in delayed insights and missed market opportunities. The absence of a centralized, automated architecture made it difficult to respond to real-time market volatility.

---

## 🎯 Project Objectives

- Automate ingestion of real-time crypto data from CoinGecko API
- Store raw JSON in Azure Data Lake (Bronze layer)
- Cleanse and structure data using Databricks and Delta Live Tables (Silver layer)
- Load business-ready data into Azure SQL Database (Gold layer)
- Visualize insights with Power BI

---

## 🧱 Architecture

The pipeline follows the Medallion Architecture:

- **Bronze Layer**: Raw data from CoinGecko API → Azure Blob
- **Silver Layer**: Cleaned data using Delta Lake and schema enforcement
- **Gold Layer**: Structured, analytics-ready data in Azure SQL for Power BI

---

## 🛠 Technology Stack

- **Azure**: Blob Storage, Data Factory, Key Vault, SQL Database
- **Databricks**: Auto Loader, Delta Lake, Delta Live Tables, Unity Catalog
- **Development**: Python, Spark, GitHub, Draw.io
- **Visualization**: Power BI
- **Source**: CoinGecko API

---

## 📁 Project Structure

```
.
├── notebooks/
│   ├── bronze_ingest.py
│   ├── silver_transform.py
│   └── gold_merge.sql
├── docs/
│   └── architecture_diagram.drawio
├── powerbi/
│   └── Crypto.pbix
├── pipelines/
│   └── delta_live_config.json
├── README.md
```

---

## 🔍 Key Features

- 🔁 Auto-ingestion via Auto Loader
- ✅ Schema enforcement and evolution
- 🔒 ACID-compliant data storage with Delta Lake
- 📊 Power BI dashboard with live insights
- ⏱ Automated processing via Databricks Jobs

---

## 📊 Dashboard Highlights

- Total Market Cap, Volume, and ROI KPIs
- Top 10 cryptocurrencies by market cap
- Volatility vs Liquidity analysis
- ROI trends over time
- Interactive filters by coin and performance metrics

---

## 🚀 How to Run

1. Clone this repository
2. Set up Azure resources: Blob Storage, Databricks, SQL DB
3. Configure paths and credentials using Key Vault
4. Run the pipeline via Databricks notebooks or jobs
5. Open Power BI file to view dashboard

---

## 🧠 Author

**Chukwunweike Stephen Osamezu**  
Data Engineer | Amdari Internship  
[LinkedIn Profile or GitHub Handle]

---

## 📜 License

MIT License – see [LICENSE](./LICENSE) for details.
