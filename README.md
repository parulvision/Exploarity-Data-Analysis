# Exploarity-Data-Analysis

## Overview
This repository presents a thorough exploratory data analysis (EDA) of the Superstore sales dataset, showcasing data science techniques in Python. The project covers data preprocessing, statistical analysis, and visualization to uncover patterns in sales, customer behavior, and product performance.

## Dataset Description
- **Source**: The `train.csv` file contains transactional data from a superstore, including fields like Order ID, Order Date, Ship Date, Ship Mode, Customer ID, Customer Name, Segment, Country, City, State, Postal Code, Region, Product ID, Category, Sub-Category, Product Name, Sales, Quantity, Discount, and Profit.
- **Size**: Approximately 9,800+ rows of sales transactions.
- **Purpose**: To analyze sales trends, customer segments, and operational efficiencies.

## Project Structure
- `Superstore Sales Analysis.ipynb`: Comprehensive Jupyter Notebook with step-by-step analysis, code, and visualizations.
- `train.csv`: Raw dataset for replication.
- `README.md`: This file with project details.

## Detailed Analysis Breakdown

### 1. Data Cleaning and Exploration
- **Null Value Handling**: Identified and filled missing postal codes with 0, converted to integer type.
- **Duplicate Check**: Verified no duplicates in the dataset.
- **Data Types**: Ensured proper types for dates and numerical fields.
- **Descriptive Statistics**: Summary of numerical columns using `df.describe()`.

### 2. Customer Analysis
- **Segmentation**: 
  - Unique segments: Consumer, Corporate, Home Office.
  - Pie chart showing distribution (Consumer: ~51%, Corporate: ~30%, Home Office: ~18%).
- **Sales per Segment**: Bar chart and pie chart of total sales by segment.
- **Customer Loyalty**: Grouped by customer ID to count orders; identified repeat customers.
- **Top Spenders**: Sorted customers by total sales; displayed top 10.

### 3. Shipping Analysis
- **Shipping Modes**: Frequency of Standard Class, Second Class, First Class, Same Day.
- **Visualization**: Pie chart of shipping mode usage.

### 4. Geographical Analysis
- **State-wise Customers and Sales**: Top states by customer count and sales (e.g., California, New York).
- **City-wise Analysis**: Top cities by customers and sales.
- **Combined State-City Sales**: Grouped analysis for deeper insights.

### 5. Product Analysis
- **Categories**: Furniture, Office Supplies, Technology.
- **Sub-Categories**: 17 unique sub-categories under the main categories.
- **Sales by Category/Sub-Category**: Bar charts and horizontal bar plots ranking by sales.
- **Top Performers**: Technology leads in sales, followed by Furniture and Office Supplies.

### 6. Sales Trends Over Time
- **Date Conversion**: Parsed 'Order Date' to datetime.
- **Yearly Sales**: Bar and line plots showing growth from 2015-2018.
- **Quarterly Sales (2018)**: Breakdown by quarters.
- **Monthly Sales (2018)**: Detailed monthly trends.
- **Overall Trends**: Monthly, quarterly, and yearly plots using period grouping.

## Visualizations Used
- **Pie Charts**: For categorical distributions (segments, shipping modes, sales by category).
- **Bar Charts**: For comparisons (sales per segment, yearly sales).
- **Line Plots**: For time series (sales trends).
- **Horizontal Bar Charts**: For ranking sub-categories.

## Technologies and Dependencies
- **Python 3.x**
- **Libraries**:
  - `pandas`: Data manipulation.
  - `numpy`: Array operations.
  - `matplotlib.pyplot`: Plotting.
- **Environment**: Jupyter Notebook for interactive execution.

## Prerequisites
- Python installed (preferably via Anaconda for easy package management).
- Jupyter Notebook: `pip install jupyter`.
- Required libraries: `pip install pandas numpy matplotlib`.

## How to Run the Project
1. **Clone the Repository**:
   ```
   git clone https://github.com/yourusername/Exploarity-Data-Analysis.git
   cd Exploarity-Data-Analysis
   ```

2. **Install Dependencies** (if not already installed):
   ```
   pip install pandas numpy matplotlib
   ```

3. **Launch Jupyter Notebook**:
   ```
   jupyter notebook
   ```
   Open `Superstore Sales Analysis.ipynb` and run cells from top to bottom.

4. **Reproduce Analysis**: Ensure `train.csv` is in the same directory. Execute cells to generate outputs and plots.

## Key Insights
- **Customer Insights**: Consumer segment is largest but Corporate has higher average sales per customer.
- **Sales Insights**: Steady annual growth; Q4 peaks in quarterly sales.
- **Product Insights**: Chairs and Phones are top sub-category sellers.
- **Geographical Insights**: West region leads in sales; New York City is top city.
- **Shipping Insights**: Standard Class dominates due to cost-effectiveness.

## Acknowledgments
- Dataset inspired by standard Superstore data on Kaggle.
- Built for educational purposes in data analysis.