# Generate Sales SQL Script

## Description
This file contains SQL scripts used to manage and update the sales table in the data warehouse. The process includes steps to extract, transform, and load sales data from staging tables into dimension and fact tables within the data warehouse.

## Key Features
- **Dimension Table Creation**: Creates and updates dimension tables for products, stores, time, and sales names.
- **Fact Table Creation**: Inserts sales data into the `fact_sales` table, ensuring that the entered data is unique and not duplicated.
- **Use of `TRUNCATE` and `INSERT`**: Empties the tables before updating data, so only the latest data is stored.
- **View Creation for Data Mart**: Creates views to facilitate access to integrated sales transaction data from various dimensions.

## File Structure
- `CREATE TABLE`: Prepares dimension and fact tables.
- `INSERT INTO`: Inserts new data into tables.
- `SELECT DISTINCT`: Ensures there are no duplicate data entries.
- `TRUNCATE`: Deletes old data before updates.
- `CREATE OR REPLACE VIEW`: Builds views for data integration.

## How to Use
1. Run this script in a SQL environment that supports PostgreSQL.
2. Ensure all staging tables are populated with relevant data before executing the script.
3. Check the results in the dimension and fact tables to ensure the data has been updated correctly.

## Contributions
Contributions for improvements or new feature additions are welcome. Please create a pull request or open an issue if you have any questions.
