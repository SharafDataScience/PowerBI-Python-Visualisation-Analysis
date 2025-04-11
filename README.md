# 📊 E-Commerce Data Analysis Projects (Brazilian Olist Dataset)

This repository contains four different data visualization and analysis designs based on the **Brazilian E-Commerce Public Dataset by Olist**. The goal is to explore market behavior, customer satisfaction, and payment trends using Python and Power BI.
Author: Abdullah Sharaf
---

## 🔗 Dataset Source

All datasets used in these projects can be found at:  
[https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

---

## Project Overview

### Design 1 – **Payment Type Comparison (Q1 2017 vs Q1 2018)**

- **Goal**: Compare total payment values by payment method (credit card, boleto, voucher, debit card).
- **Tools**: Power BI  
- **Used Datasets**:
  - `olist_order_payments_dataset.csv`
  - `olist_orders_dataset.csv`
- **Timeframe Filter**: January–March 2017 & 2018
- **Insight**: Credit cards dominated both years. Steady growth across all payment types observed.
- **Action Level**:
  - High: Discover payment trends
  - Mid: Lookup preferences
  - Low: Compare value by payment method

---

### Design 2 – **Sales Outliers in Top Categories (Nov 2017)**

- **Goal**: Identify outlier days for top product categories in sales.
- **Tools**: Python (Altair)  
- **Used Datasets**:
  - `olist_order_payments_dataset.csv`
  - `olist_orders_dataset.csv`
  - `olist_products_dataset.csv`
  - `olist_order_items_dataset.csv`
- **Focus Month**: November 2017 (Black Friday)
- **Top Categories**:
  - `cama_mesa_banho` (bed, table, and bath)
  - `moveis_decoracao` (furniture and decoration)
- **Insight**: Nov 24 (Black Friday) had the highest sales spike in both categories.
- **Action Level**:
  - High: Detect outlier dates
  - Mid: Lookup daily trends
  - Low: Compare category performance

---

### Design 3 – **Geographic Order Distribution (2018)**

- **Goal**: Identify regions with the highest number of e-commerce orders.
- **Tools**: Python  
- **Used Datasets**:
  - `olist_geolocation_datasett.csv`
  - `olist_orders_datasett.csv`
  - `olist_customers_datasett.csv`
- **Focus Year**: 2018
- **Insight**: São Paulo and Rio de Janeiro were top-performing cities, with strong trust in e-commerce.
- **Action Level**:
  - High: Spot geographic outliers
  - Mid: Lookup by location
  - Low: Compare neighboring regions

---

### Design 4 – **Review Score Trends vs Order Volume (2017–2018)**

- **Goal**: Analyze review score changes during seasonal order peaks.
- **Tools**: Power BI  
- **Used Datasets**:
  - `olist_order_reviews_datasett.csv`
  - `olist_orders_datasett.csv`
- **Timeframe**: Feb 2017 – Apr 2018
- **Insight**: Review scores dipped slightly during high order volumes (e.g., holidays).
- **Action Level**:
  - High: Discover seasonal trends
  - Mid: Lookup reviews & order timelines
  - Low: Compare review dependency on volume

---

## ⚙️ Setup & Instructions

For Python Projects (Design 2 & 3):
- Download the datasets from Kaggle
- Update dataset paths in the script, for example:
  ```python
  df = pd.read_csv("path/to/olist_orders_dataset.csv")
