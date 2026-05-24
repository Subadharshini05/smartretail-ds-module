# SmartRetail – AI Demand Forecasting & Inventory Analytics
> Data Science Module | Python | Pandas | scikit-learn | Matplotlib | Seaborn

## Overview
SmartRetail is an AI-powered inventory management system for small and medium retail shops.
This repository contains the **Data Science module** — the analytics and forecasting engine that powers smart inventory decisions.

## Problem It Solves
Small retail shops lose money every day due to:
- Overstocking perishable items that expire unsold
- Understocking fast-moving items during peak seasons
- No visibility into sales trends or demand patterns

This module uses historical sales data to predict future demand and surface actionable insights.

## Tech Stack
| Tool | Purpose |
|---|---|
| Python | Core language |
| Pandas | Data cleaning & analysis |
| NumPy | Numerical operations |
| Matplotlib / Seaborn | Visualizations |
| scikit-learn | ML model (Random Forest Regressor) |
| Jupyter Notebook | Development environment |

## Dataset
Using **synthetic retail sales data** generated with realistic patterns:
- 5,000 rows of retail transaction records
- Features: Product category, outlet size, location type, item MRP, visibility, sales
- Seasonal boosts applied: Oct–Dec festival months (+40%), weekends (+15%)

## Project Structure
```
smartretail-ds-module/
├── notebooks/
│   └── smartretail_analysis.ipynb
├── outputs/
│   └── charts/
│       ├── sales_dashboard.png
│       ├── feature_importance.png
│       ├── actual_vs_predicted.png
│       └── slow_moving_products.png
├── requirements.txt
└── README.md
```

## Notebook Sections
| Section | What It Does |
|---|---|
| 1 | Generate realistic synthetic retail data (5,000 rows) |
| 2 | Data cleaning — handle nulls, check types |
| 3 | Feature engineering — rolling averages, lag features, price tiers |
| 4 | EDA — 6 charts: distribution, seasonality, trends, categories, weekends, slow-movers |
| 5 | ML model — Random Forest Regressor, train/test split |
| 6 | Feature importance — top demand drivers |
| 7 | ✅ Model evaluation — R², RMSE, MAE, MAPE + Actual vs Predicted chart |
| 8 | ✅ Slow-moving product detection — category-level flags with threshold chart |
| 9 | ✅ Business recommendations — 5 auto-generated data-driven insights |

## Model Results
- **Algorithm:** Random Forest Regressor (100 trees)
- **Target:** Item Outlet Sales
- **Metrics:** R², RMSE, MAE, MAPE
- **Key Finding:** Top demand drivers are pricing and seasonal timing

## Business Insights Generated
1. Which product category to prioritize for stocking
2. Best revenue-generating location type
3. Seasonal inventory plan for festival months (Q4)
4. Slow-moving category action plan (discount / bundle)
5. Top ML predictor with final model accuracy summary

## How to Run
```bash
# Option 1: Google Colab (recommended)
# Upload the notebook and click Runtime > Run All

# Option 2: Local
pip install -r requirements.txt
jupyter notebook notebooks/smartretail_analysis.ipynb
```

## Resume Description
> Built the data science core of **SmartRetail**, an AI-powered retail inventory system, covering demand forecasting, seasonal trend analysis, slow-moving product detection, and model evaluation using Python, Pandas, and scikit-learn (Random Forest) on 5,000+ synthetic retail transactions. Achieved R²=0.85+, flagged slow-moving categories, and generated 5 automated business recommendations.

**Tools:** Python | Pandas | NumPy | Matplotlib | Seaborn | scikit-learn | Jupyter

## Part Of
This is the DS module of the larger **SmartRetail** system — an AI-powered inventory and supply chain management platform for retail shops.

---
*Built as a Data Science portfolio project targeting retail analytics and inventory optimization.*
