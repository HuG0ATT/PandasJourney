# Project 01: Basic DataFrame Exploration with Sales Data

<br>

## Overview
This project is the first in a series of 50 hands-on pandas projects aimed at mastering pandas, a powerful Python library for data manipulation and analysis. Designed for beginners, this project focuses on fundamental DataFrame operations using a small retail sales dataset. The goal is to load, inspect, filter, and summarize data while learning key pandas functions and concepts like DataFrames, Series, indexing, and filtering.

<br>

## Dataset
The dataset, `sales_data.csv`, contains sales records for a small retail store with the following columns:
- `order_id`: Unique identifier for each order
- `product`: Product name
- `category`: Product category, e.g., Electronics, Clothing
- `quantity`: Number of items sold
- `price`: Price per item in USD
- `order_date`: Date of the order

<br>

### Generating the Dataset
Run the following Python code to create `sales_data.csv` in your working directory:

```python
import pandas as pd

data = {
    'order_id': [1, 2, 3, 4, 5, 6, 7, 8],
    'product': ['Laptop', 'T-shirt', 'Headphones', 'Jacket', 'Mouse', 'Shoes', 'Monitor', 'Keyboard'],
    'category': ['Electronics', 'Clothing', 'Electronics', 'Clothing', 'Electronics', 'Clothing', 'Electronics', 'Electronics'],
    'quantity': [1, 3, 2, 1, 5, 2, 1, 4],
    'price': [999.99, 19.99, 49.99, 89.99, 29.99, 59.99, 199.99, 39.99],
    'order_date': ['2023-01-15', '2023-01-16', '2023-01-16', '2023-01-17', '2023-01-18', '2023-01-18', '2023-01-19', '2023-01-20']
}

df = pd.DataFrame(data)
df.to_csv('sales_data.csv', index=False)
```

<br>

## Objectives
- Learn fundamental pandas concepts: DataFrames, Series, indexing, filtering, and aggregation.
- Master key pandas functions: `read_csv()`, `head()`, `dtypes`, `describe()`, filtering, column creation, `sum()`, and `mean()`.
- Perform basic data exploration and manipulation on a real-world dataset.

<br>

## Tasks
The project involves the following tasks:
1. **Load the Data**: Read `sales_data.csv` into a pandas DataFrame.


2. **Inspect the Data**:
   - Display the first 5 rows.
   - Check data types of each column.
   - Generate summary statistics for numerical columns.


3. **Filter the Data**:
   - Create a DataFrame for orders in the "Electronics" category.
   - Create a DataFrame for orders with quantity > 2.


4. **Compute a New Column**:
   - Add a `total_sales` column by multiplying `quantity` and `price`.


5. **Summarize Sales**:
   - Calculate the total sales (sum of `total_sales`).
   - Find the average price of products in the "Clothing" category.

<br>

## Requirements
- Python 3.x
- pandas (`pip install pandas`)

<br>

## Learning Outcomes
By completing this project, you will:
- Understand how to load and inspect data with pandas.
- Gain proficiency in filtering and creating new columns.
- Learn to compute summary statistics using aggregation functions.
- Build a foundation for more complex pandas operations in future projects.

<br>

## Next Steps
This project is followed by Project 02, which introduces grouping and aggregation with `groupby()` using a new dataset to explore more advanced pandas functionality.

<br>

## License
This project is licensed under the MIT License.
