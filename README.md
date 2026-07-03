# instamart_repo
Analyzing data of instamart with databricks

# Instacart Market Basket Analysis — Medallion Architecture

A Databricks data pipeline implementing Bronze/Silver/Gold architecture 
on the Instacart Market Basket Analysis dataset (Kaggle).

## Architecture
- **Bronze**: Raw ingestion of 6 source CSVs (orders, products, aisles, 
  departments, order_products__prior, order_products__train)
- **Silver**: Data quality enforcement (NOT NULL constraints, deduplication)
- **Gold**: Enriched fact tables and business-ready aggregates 
  (reorder rates, product affinity/market basket pairs, customer 
  purchase behavior, order timing patterns)

## Tech stack
- Databricks (Delta Lake, Unity Catalog)
- SQL 
- Source data: Kaggle - Instacart Market Basket Analysis

## Project structure
notebooks/ — Bronze, Silver, Gold pipeline notebooks
conf/ — shared configuration (catalog/schema names, paths)
