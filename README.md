# Kenya Mobile Money Analysis

Exploratory analysis of 6,000 Kenyan mobile money transactions from 2024 (M-Pesa and Airtel Money), done in Python with pandas.

## Dataset

`kenya_mobile_money_transactions.csv` has 16 columns, including transaction time, customer details, county, channel, transaction type, amount, fee and status. The `merchant_category` column is empty for 3,551 rows because only merchant payments (Buy Goods, Pay Bill) have a category. All analysis uses **completed** transactions only.

The data file is not included in this repository. To run the notebook, place the CSV on your machine and update the file path in the "Load the dataset" cell.

## Questions answered

1. **Monthly fee revenue and growth:** Fee revenue per month with month-over-month % change. May grew fastest (+11.2%) and June fell the most (-14.8%).
2. **Peak transaction hours:** A weekday by hour matrix of transaction counts. The busiest hour was Wednesday at 9 am, with 69 transactions.
3. **Top customers per county:** The top 3 customers by total amount transacted in each county, ranked within the county.
4. **7-day rolling volume:** Daily transaction counts with a 7-day rolling average. Volume exceeded 1.5 times its rolling average on 4 days.
5. **RFM segmentation:** Recency, Frequency and Monetary value per customer, each scored 1 to 5 by quintile. Customers scoring 5 on all three are labelled "Champions".

## Tools

Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

## How to run

1. Install the libraries: `pip install pandas numpy matplotlib seaborn`
2. Open `analysis.ipynb` in Jupyter or VS Code.
3. Update the CSV path in the data loading cell.
4. Run all cells from top to bottom.

## Files

- `analysis.ipynb`: the full analysis
- `README.md`: this file
