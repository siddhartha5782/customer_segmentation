# Customer Segmentation

## Overview

This project focuses on customer segmentation using transaction data to identify distinct customer groups based on their purchasing behaviors. Understanding these segments can help businesses tailor marketing strategies and improve customer satisfaction.

## Dataset

The dataset used for this analysis is `int_online_tx.csv`, which contains transaction records from an online retailer. Each entry includes details such as:

- **Transaction ID**: Unique identifier for each transaction.
- **Customer ID**: Unique identifier for each customer.
- **Transaction Date**: The date of purchase.
- **Purchase Amount**: The amount spent by the customer.

## Analysis Process

The main analysis is conducted in the `Customer_Segmentation.ipynb` Jupyter Notebook, which includes the following steps:

1. **Data Preprocessing**
   - Load the dataset and explore its structure.
   - Handle missing values and remove duplicate entries.
   - Convert transaction dates to appropriate datetime formats.

2. **Feature Engineering**
   - Compute **Recency** (days since last purchase).
   - Compute **Frequency** (total number of purchases).
   - Compute **Monetary** (total amount spent).
   - Create an RFM (Recency, Frequency, Monetary) table.

3. **Clustering**
   - Normalize the RFM values for better performance.
   - Apply **K-Means Clustering** to segment customers.
   - Determine the optimal number of clusters using the **Elbow Method**.

4. **Visualization**
   - Plot the distribution of RFM values.
   - Visualize customer segments to understand their characteristics.

## Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas** (Data manipulation)
- **NumPy** (Numerical operations)
- **Matplotlib** & **Seaborn** (Data visualization)
- **Scikit-learn** (Clustering and machine learning)

## Installation

To run this project on your local machine, ensure you have the following dependencies installed.

### Install Required Packages

Run the following command in your terminal:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
