# Amazon Sales Data Analysis 📊

A comprehensive Exploratory Data Analysis (EDA) project on Amazon sales data, uncovering insights into sales performance, customer behavior, product trends, and operational efficiency using Python.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Objectives](#objectives)
- [Dataset Description](#dataset-description)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Data Cleaning & Preprocessing](#data-cleaning--preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Key Insights](#key-insights)
- [Business Recommendations](#business-recommendations)
- [Getting Started](#getting-started)
- [Author](#author)

---

## Project Overview

This project performs end-to-end Exploratory Data Analysis on Amazon sales transaction data. Raw data is cleaned, preprocessed, and visualized to surface actionable business insights around revenue trends, top-performing categories, regional demand, and order fulfillment efficiency.

---

## Objectives

- Analyze overall sales trends over time
- Identify top-performing product categories
- Understand customer purchasing behavior
- Explore geographical distribution of sales
- Evaluate operational performance through order status and cancellation rates
- Generate actionable business recommendations

---

## Dataset Description

The dataset contains Amazon sales transaction records with the following attributes:

| Column | Description |
|---|---|
| Order ID | Unique identifier for each order |
| Date | Order placement date |
| Status | Current status of the order |
| Category | Product category |
| Size | Product size variant |
| Quantity | Number of units ordered |
| Amount | Transaction value |
| Currency | Currency of the transaction |
| Fulfillment | Fulfillment method used |
| City / State / Postal Code | Customer location details |

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data cleaning and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualizations |
| Jupyter Notebook | Interactive development environment |

---

## Project Structure

```
amazon-sales-eda/
│
├── data/
│   ├── raw/                  # Original dataset
│   └── processed/            # Cleaned datasets
│
├── notebooks/
│   └── amazon_sales_eda.ipynb   # Main analysis notebook
│
├── visuals/                  # Exported charts and plots
│
├── requirements.txt
└── README.md
```

---

## Data Cleaning & Preprocessing

The raw dataset required several preprocessing steps before analysis:

- **Missing values** — handled in key columns using imputation or removal strategies
- **Date formatting** — standardized date fields to enable time-series analysis
- **Invalid entries** — removed records with zero or null transaction amounts
- **Feature engineering** — extracted `month` and `day_of_week` fields for temporal analysis
- **Dataset segmentation** — split into two subsets:
  - **Sales Dataset** — filtered for revenue-focused analysis
  - **Full Dataset** — retained for operational and behavioral insights

---

## Exploratory Data Analysis

The analysis covers five core dimensions:

1. **Sales Trend Analysis** — Monthly revenue patterns and peak period identification
2. **Product Performance** — Category-wise breakdown of sales volume and revenue
3. **Geographical Distribution** — State and city-level sales heatmaps
4. **Customer Behavior** — Order patterns by day of the week
5. **Operational Analysis** — Order status breakdown and cancellation rate evaluation

---

## Key Insights

| Area | Finding |
|---|---|
| 📅 Peak Sales Month | April recorded the highest sales, followed by a decline |
| 👕 Top Category | T-shirts are the best-performing product category |
| 🗺️ Leading States | Maharashtra, Karnataka, and Telangana dominate sales |
| 🏙️ Top Cities | Bengaluru, Hyderabad, and Mumbai lead among metro cities |
| 📆 Busiest Day | Sunday has the highest order volume |
| 📆 Slowest Day | Thursday records the lowest order volume |
| ✅ Fulfillment Rate | Over 85% order completion rate — indicating strong operations |

---

## Business Recommendations

- **Double down on top categories** — Invest in inventory and marketing for T-shirts and other high-performing segments
- **Re-evaluate low performers** — Audit and consider phasing out underperforming product lines
- **Target high-value regions** — Focus advertising spend on Maharashtra, Karnataka, and Telangana
- **Boost midweek sales** — Run promotions on Tuesdays–Thursdays to reduce the order volume dip
- **Sustain fulfillment quality** — Maintain and monitor the processes driving the >85% completion rate

---

## Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Run the Analysis

```bash
# Clone the repository
git clone https://github.com/your-username/amazon-sales-eda.git
cd amazon-sales-eda

# Launch Jupyter Notebook
jupyter notebook notebooks/amazon_sales_eda.ipynb
```

---

## Author

**Simardeep Kaur**

---
