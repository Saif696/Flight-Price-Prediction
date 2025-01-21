# Exploratory Data Analysis (EDA) Project: Online Retail Dataset

## Project Overview
This project involves performing Exploratory Data Analysis (EDA) on the Online Retail dataset to extract meaningful insights and patterns. The dataset contains transactional data from a UK-based online retail store, spanning from December 1, 2010, to December 9, 2011. The goal is to analyze customer purchasing behavior, identify sales trends, and uncover insights for better decision-making.

---

## Dataset Information
- **Source**: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail)
- **Records**: 541,909 transactions
- **Period Covered**: December 1, 2010 – December 9, 2011
- **Features**:
  - **InvoiceNo**: Unique identifier for each transaction (starts with 'C' for cancellations).
  - **StockCode**: Unique identifier for each product.
  - **Description**: Product description.
  - **Quantity**: Number of items purchased per transaction.
  - **InvoiceDate**: Date and time of the transaction.
  - **UnitPrice**: Price per unit of the product (in sterling £).
  - **CustomerID**: Unique identifier for each customer.
  - **Country**: Customer’s country of residence.

---

## Project Objectives
1. Understand the dataset structure and contents.
2. Perform data cleaning to ensure accuracy and consistency.
3. Conduct detailed analysis to:
   - Explore sales trends.
   - Identify best-selling products and frequent customers.
   - Analyze customer purchasing behavior.
   - Explore country-specific performance.
4. Visualize key insights using graphs and charts.
5. Document the findings for portfolio presentation.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**:
  - Pandas
  - NumPy
  - Matplotlib
  - Seaborn
- **IDE**: Jupyter Notebook
- **Version Control**: GitHub

---

## Steps
1. **Data Overview**:
   - Inspect structure, shape, and summary statistics.
   - Identify unique values and data types.
2. **Data Cleaning**:
   - Handle missing values and duplicates.
   - Address anomalies or outliers.
3. **Exploration**:
   - Analyze individual features and relationships.
   - Perform time-series analysis.
   - Study customer demographics and purchase patterns.
4. **Visualization**:
   - Plot sales trends, distributions, and correlations.
   - Visualize geographic performance.
5. **Documentation**:
   - Record findings and visualizations.
   - Present insights in an organized format.

---

## Key Findings
1. **Data Cleaning and Preparation**:
   - Removed rows with missing `Description` values (~0.42% of the data).
   - Addressed duplicate records, eliminating 196 duplicate rows.
   - Added a derived column `TotalSales` to calculate total revenue for each transaction.

2. **Sales Trends**:
   - Daily sales trends highlighted consistent patterns with occasional spikes, potentially due to seasonal events or promotions.
   - A detailed time-series plot revealed peak sales periods.

3. **Product Performance**:
   - Identified the top 10 products by revenue. These products significantly contributed to the total sales, with some high-priced items leading in revenue despite lower quantities sold.
   - Created a bar chart to visually represent the top-performing products.

4. **Anomalies**:
   - Investigated anomalies where high quantities sold resulted in low total revenue. These anomalies were attributed to low-priced products sold in bulk, such as small decorations or accessories.
   - Detailed transaction-level analysis uncovered specific examples of such anomalies, providing insights into bulk sales dynamics.

5. **Insights**:
   - High-priced, low-quantity items are key revenue drivers.
   - Bulk sales with low unit prices contribute less to revenue but represent significant volumes.

---

## Deliverables
1. Cleaned dataset.
2. Visualizations highlighting key insights.
3. A detailed report documenting findings.
4. GitHub repository showcasing the project.

---

## How to Run the Project
1. Clone the repository.
2. Install the required Python libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the Jupyter Notebook and execute the steps sequentially.

---

## Future Scope
- Develop predictive models based on transactional data.
- Implement recommendation systems for customers.
- Extend analysis to incorporate external data, such as holidays or marketing campaigns.

---

## Author
This project is part of my portfolio building as a Data Analyst/Data Scientist.

