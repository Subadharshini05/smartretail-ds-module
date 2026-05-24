# SmartRetail: Retail Demand Forecasting and Inventory Analysis

This project is a small data science case study built to explore how sales patterns can be analyzed for demand forecasting and inventory-related decisions.

I created a synthetic retail dataset and used it to practice the full workflow: data cleaning, feature engineering, exploratory analysis, model building, and interpretation of results.

## Project goal
The main goal of this project was to answer a few practical retail questions:

- Which product categories sell better on average?
- Are there visible seasonal or weekend sales patterns?
- Can we build a baseline model to predict item sales?
- Which categories look relatively slow-moving based on average sales?

## Dataset
The dataset used in this notebook is **synthetically generated** for learning purposes. It contains 5,000 retail transaction records with fields such as:

- Date
- Product category
- Outlet size
- Location type
- Item visibility
- Item MRP
- Item sales
- Time-based fields such as month, quarter, and weekend flag

Because the data is synthetic, the results should be treated as a practice exercise, not as a production-ready retail forecasting system.

## What the notebook covers
The notebook includes the following steps:

1. Generate and inspect retail transaction data
2. Clean missing values and prepare the dataset
3. Create additional features such as rolling averages, lag values, and price tiers
4. Explore patterns using charts and summary analysis
5. Train a Random Forest regression model to predict sales
6. Check feature importance
7. Evaluate the model using R², RMSE, MAE, and MAPE
8. Identify slow-moving categories based on average sales
9. Write practical observations from the results

## Main results
A Random Forest regressor was used as a baseline model for predicting item sales.

Results from the notebook:

- R² score: 0.8721
- RMSE: 643.21
- MAE: 509.87
- MAPE: 24.31%

Some patterns observed in the data:

- Sales increase during the Oct–Dec period
- Weekend sales are slightly higher than weekday sales
- Rolling sales averages are among the strongest predictors in the model
- One category appears slower-moving than the rest based on average sales

## Project structure
```text
smartretail-ds-module/
├── notebooks/
│   └── smartretail_analysis.ipynb
├── outputs/
│   └── charts/
├── requirements.txt
└── README.md
```

## Tools used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- scikit-learn
- Jupyter Notebook

## How to run
1. Clone the repository
2. Install dependencies with `pip install -r requirements.txt`
3. Open the notebook in Jupyter or Google Colab
4. Run cells in order

```bash
git clone https://github.com/Subadharshini05/smartretail-ds-module
cd smartretail-ds-module
pip install -r requirements.txt
jupyter notebook
```

## Limitations
- The dataset is synthetic, so patterns are simulated rather than collected from real stores
- The model is a baseline, not a production forecasting pipeline
- No hyperparameter tuning or time-series specific method was used
- Business observations are based only on the generated data in this notebook

## Why I built this
I built this project to practice end-to-end data science work in a way that feels practical and easy to explain. Instead of only training a model, I wanted the notebook to connect the analysis to simple retail decisions — stock planning, sales patterns, and identifying slower-moving products.
