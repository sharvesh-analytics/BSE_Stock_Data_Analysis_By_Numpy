# BSE Stock Market Data Analysis (NumPy Core Practice)

## 📌 Overview
This repository contains a Python-based data analytics practice module focused on extracting financial insights using **NumPy**. It serves as a foundational component for a larger project aimed at downloading, merging, and analyzing BSE Sensex CSV files. 

 To practice purely numerical computations without relying on Pandas, this module uses a custom 30-day simulated dataset (`AgriExport_BSE_StockData.csv`) representing an agricultural export company to calculate real-world market metrics.

## 🚀 Key Features & Operations Learned
This Jupyter Notebook demonstrates how to process raw financial data efficiently using NumPy's highly optimized array operations:

*   **Data Ingestion:** Loading specific columns from CSVs directly into 2D NumPy arrays using `np.genfromtxt`, bypassing text/date headers.
*   **Array Slicing:** Extracting targeted 1D arrays (e.g., isolating Closing Prices or Trading Volumes) using `[:, index]`.
*   **Statistical Analysis:** Calculating market volatility, average prices, and maximums using `np.mean()`, `np.max()`, and `np.std()`.
*   **Boolean Masking:** Filtering datasets conditionally without loops (e.g., isolating days with trading volumes strictly > 40,000).
*   **Vectorized Operations:** Executing fast, element-wise arithmetic across entire arrays to calculate metrics like daily price fluctuations.
*   **Financial Metrics Calculation:** 
    *   Computing **Daily Percentage Returns** `((Close - Open) / Open) * 100`.
    *   Calculating **Total Traded Value** (Money Flow) by multiplying Volume and Closing Price arrays.
*   **Index Tracking:** Using `np.argmax()` to locate the exact row/day when the stock hit its peak price and retrieving the corresponding full day's data.

## 🛠️ Technologies Used
*   **Language:** Python 3.x
*   **Libraries:** NumPy
*   **Environment:** Jupyter Notebook

## 📂 Repository Structure
*   `Stock_Analysis_NumPy.ipynb`: The main Jupyter Notebook containing the step-by-step code and theoretical explanations.
*   `AgriExport_BSE_StockData.csv`: The simulated 30-day stock market dataset used for analysis (includes Open, High, Low, Close, and Volume).

