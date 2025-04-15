
# 🛒 Task 1 : Data Cleaning and Preprocessing

This project focuses on basic exploratory data analysis (EDA) of a sales dataset. It involves reading, displaying, and checking for missing data in the dataset.

## 📂 Dataset

The dataset used is `Sales Data.csv`, which contains transaction-level data for various products sold in different cities.

### Columns Included:
- `Order ID`
- `Product`
- `Quantity Ordered`
- `Price Each`
- `Order Date`
- `Purchase Address`
- `Month`
- `Sales`
- `City`
- `Hour`

## 📊 Task 1 - Initial Exploration

### ✅ Steps Performed:
1. **Read the CSV File**:
   ```python
   import pandas as pd
   data = pd.read_csv("Sales Data.csv")
   data.head()
   ```
   This loads the sales data into a DataFrame and displays the first five rows.

2. **Check for Missing Values**:
   ```python
   miss_values = data.isnull().sum()
   miss_values
   ```
   Output showed that there are no missing values in the dataset.

### ✅ Sample Output:

| Order ID | Product               | Quantity Ordered | Price Each | Order Date        | City           | Hour |
|----------|------------------------|------------------|-------------|-------------------|----------------|------|
| 295665   | Macbook Pro Laptop     | 1                | 1700.00     | 30-12-2019 00:01  | New York City  | 0    |
| 295666   | LG Washing Machine     | 1                | 600.00      | 29-12-2019 07:03  | New York City  | 7    |
| 295667   | USB-C Charging Cable   | 1                | 11.95       | 12-12-2019 18:21  | New York City  | 18   |

## 🛠 Tools Used
- Python 3.9.6
- pandas

## 📁 File Structure
```
├── Sales Data.csv
├── task1_sales_analysis.ipynb
└── README.md
```

## 🚀 Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sales-data-analysis.git
   cd sales-data-analysis
   ```

2. Install the required libraries:
   ```bash
   pip install pandas
   ```

3. Run the notebook using Jupyter or any compatible environment.

