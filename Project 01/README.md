# 📊 Project 01 - Exploring a Simple Sales Dataset

<br>

## 🎯 Goal
Learn the **basics** of Pandas DataFrames:  
- Load a dataset  
- Explore its structure  
- Perform simple transformations and aggregations  

<br>

## 📂 Dataset
File: `sales.csv`  

### Columns
- `transaction_id` → Unique identifier for each transaction  
- `customer_id` → Identifier of the customer making the purchase  
- `product` → Name of the product purchased (e.g., Apple, Banana, Orange)  
- `quantity` → Number of units purchased in the transaction  
- `price` → Price per unit of the product  
- `date` → Date of the transaction (YYYY-MM-DD format)  

<br>

## 📝 Tasks
1. Load the CSV into a Pandas DataFrame.  
2. Display the first 5 rows.  
3. Inspect the columns, shape, and data types.  
4. Create a new column `total_sales = quantity * price`.  
5. Filter transactions where `product == "Apple"`.  
6. Calculate the **total revenue**.  
7. Count the number of unique customers.  
8. Group by `customer_id` and calculate their total purchases.  

<br>

## 🎁 Bonus Challenges
- Find the **product with the highest revenue**.  
- Find the **customer who spent the most**.  
- Find the **day with the highest sales**.  

<br>

## 🔑 Pandas Functions Covered
- `pd.read_csv()`  
- `.head()`  
- `.info()`, `.columns`, `.shape`  
- Creating new columns: `df["new_col"] = ...`  
- Filtering with boolean indexing and `.query()`  
- `.sum()`, `.nunique()`  
- `.groupby()` + `.agg()`  
- `.nlargest()`, `.idxmax()`  

<br>

## 📚 Key Concepts
- **DataFrame**: Pandas’ main table structure (rows + columns).  
- **Series**: A single column of a DataFrame.  
- **Indexing**: Selecting/filtering rows and columns.  
- **Vectorized operations**: Perform calculations directly on columns.  
- **Aggregation**: Summarizing groups with `.sum()`, `.mean()`...  
