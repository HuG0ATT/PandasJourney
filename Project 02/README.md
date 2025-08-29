# Project 02: Grouping and Aggregating Sales Data by Category

<br>

## Overview
This project is the second in a series of 50 hands-on pandas projects aimed at mastering pandas, a powerful Python library for data manipulation and analysis. Designed for beginner-to-intermediate learners, this project builds on basic DataFrame operations from Project 01 by introducing grouping and aggregation with `groupby()`. It involves loading, inspecting, grouping, filtering, and sorting a retail sales dataset, with optional visualizations to enhance understanding.

<br>

## Dataset
The dataset, `store_sales.csv`, contains sales records for a retail store across multiple categories. It includes the following columns:
- `order_id`: Unique identifier for each order
- `product`: Product name
- `category`: Product category, e.g., Electronics, Clothing, Books
- `quantity`: Number of items sold
- `price`: Price per item in USD
- `order_date`: Date of the order

<br>

### Generating the Dataset
Run the following Python code to create `store_sales.csv` in your working directory:

```python
import pandas as pd

data = {
    'order_id': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
    'product': ['Laptop', 'T-shirt', 'Headphones', 'Jacket', 'Book A', 'Mouse', 'Shoes', 'Monitor', 'Book B', 'Keyboard'],
    'category': ['Electronics', 'Clothing', 'Electronics', 'Clothing', 'Books', 'Electronics', 'Clothing', 'Electronics', 'Books', 'Electronics'],
    'quantity': [1, 2, 3, 1, 4, 2, 3, 1, 5, 2],
    'price': [999.99, 19.99, 49.99, 89.99, 14.99, 29.99, 59.99, 199.99, 9.99, 39.99],
    'order_date': ['2023-02-01', '2023-02-01', '2023-02-02', '2023-02-02', '2023-02-03', '2023-02-03', '2023-02-04', '2023-02-04', '2023-02-05', '2023-02-05']
}

df = pd.DataFrame(data)
df.to_csv('store_sales.csv', index=False)
```

<br>

## Objectives
- Learn grouping and aggregation with `groupby()` to summarize data by category.
- Reinforce pandas concepts: DataFrames, Series, filtering, sorting, and column creation.
- Master key pandas functions: `read_csv`, `head`, `dtypes`, `groupby`, `sum`, `mean`, `sort_values`, `nlargest`.
- Optionally visualize grouped results using `seaborn` and `matplotlib`.

<br>

## Tasks
The project involves the following tasks:


1. **Load and Inspect the Data**:
   - Load `store_sales.csv`, converting `order_date` to datetime and `category`/`product` to categorical types.
   - Display the first 5 rows.
   - Check data types of each column.


2. **Group and Aggregate by Category**:
   - Group by `category` and calculate the total `quantity` sold.
   - Group by `category` and calculate the average `price`.


3. **Filter and Summarize**:
   - Create a DataFrame with orders where `price` > 50.
   - Calculate the total sales value (quantity * price) for these orders.


4. **Sort and Display**:
   - Sort total quantity by category in descending order.
   - Display the top 2 categories by total quantity sold.

<br>

## Requirements
- Python 3.x
- pandas (`pip install pandas`)
- seaborn (`pip install seaborn`, optional for visualizations)
- matplotlib (`pip install matplotlib`, optional for visualizations)

<br>

## Learning Outcomes
By completing this project, you will:
- Understand how to group and aggregate data with `groupby()`.
- Gain proficiency in filtering, sorting, and creating new columns.
- Learn to combine pandas operations for data analysis.
- Optionally visualize results to enhance data interpretation.
- Build a foundation for advanced pandas operations like multi-column grouping and joins.

<br>

## Next Steps
This project is followed by Project 03, which introduces multi-column grouping and joins (`merge()`) using a new dataset to explore more complex pandas functionality.

<br>

## License
This project is licensed under the MIT License.
