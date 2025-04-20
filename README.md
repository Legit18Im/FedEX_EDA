# 📦 FedEx Shipping Data - Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project focuses on performing **Exploratory Data Analysis (EDA)** on a dataset provided by FedEx to identify key patterns, trends, and insights in their shipping process. The objective is to understand the factors affecting delays, cost distribution, and operational behavior to make data-driven business recommendations for improvement.

---

## 🎯 Problem Statement

FedEx frequently faces operational inefficiencies such as **shipment delays**, **insurance surges**, and **irregular vendor schedules**. These issues can lead to increased costs, dissatisfied clients, and logistical bottlenecks.

### ✅ Business Objective:
To analyze the shipping data and:
- Uncover hidden patterns contributing to **delays and inefficiencies**
- Understand **cost drivers** like unit price, pack price, and insurance
- Suggest **recommendations** based on correlation, trends, and frequency analysis

---

## 🧾 Dataset Description

The dataset contains information about:
- Item quantity, value, insurance, and price
- Purchase order and quotation dates
- Weekday patterns and delivery delays

**Key Columns:**
- `line_item_quantity`, `line_item_value`, `unit_price`, `line_item_insurance_usd`
- `po_sent_to_vendor_date`, `pq_first_sent_to_client_date`
- `delay_days`, `pack_price`, and associated weekday/date components

---

## 🔍 EDA Tasks Performed

- Displayed `head()`, `tail()`, and `info()` to understand structure
- Checked for missing/null values and cleaned the dataset
- Converted date columns to datetime objects and extracted day, month, year, and weekday
- Created a **data dictionary** to describe features
- Applied `describe()` for statistical summaries

---

## 📊 Visualizations

> At least **five different types of visualizations** were used:

1. **Histogram** – Distribution of `line_item_value`
2. **Box Plot** – Comparison of `unit_price` vs. `line_item_insurance_usd`
3. **Bar Chart** – Shipment frequency by `weekday`
4. **Pair Plot** – Relationships among numeric variables
5. **Correlation Heatmap** – Identify linear relationships among features

---

## 📌 Key Insights

- `line_item_value` is strongly correlated with `line_item_insurance_usd` (correlation ~0.96)
- Shipment delays are not significantly correlated with cost-related features
- Most shipments are dispatched mid-week; weekends see low activity
- Insurance costs tend to rise sharply with item value

---

## 💡 Business Recommendations

- Revise insurance calculation models to consider item category, not just value
- Optimize shipment scheduling to avoid delay-prone days
- Automate vendor coordination to reduce lag in processing POs

---

## 📂 Project Structure

