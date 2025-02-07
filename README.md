# Home Sales Analysis  

## Instructions  

This project analyzes home sales data using PySpark and SparkSQL to answer key real estate questions.  

### Steps to Complete:  

1. **Rename File:**  
   - Rename `Home_Sales_starter_code.ipynb` to `Home_Sales.ipynb`.  

2. **Set Up PySpark:**  
   - Import necessary PySpark SQL functions.  

3. **Load Data:**  
   - Read `home_sales_revised.csv` from the provided AWS S3 bucket into a PySpark DataFrame.  

4. **Create Temporary Table:**  
   - Register the DataFrame as a temporary table named `home_sales`.  

5. **Run Queries Using SparkSQL:**  
   - Find the **average price** of four-bedroom houses sold per year (rounded to two decimals).  
   - Find the **average price** of homes with **three bedrooms and three bathrooms**, grouped by year built.  
   - Find the **average price** of homes with **three bedrooms, three bathrooms, two floors, and ≥2,000 sqft**, grouped by year built.  
   - Find the **average home price per "view" rating** where the average price is **≥ $350,000** and determine the runtime.  

6. **Optimize Performance with Caching:**  
   - Cache the `home_sales` temporary table.  
   - Verify caching.  
   - Re-run the last query on cached data and compare runtime.  

7. **Partition and Parquet Conversion:**  
   - Partition the dataset by `date_built` and store as **parquet**.  
   - Create a temporary table from parquet data.  
   - Re-run the last query on the parquet table and compare runtime.  

8. **Clean Up Resources:**  
   - Uncache and verify the removal of the `home_sales` temporary table.  

9. **Final Steps:**  
   - Download `Home_Sales.ipynb`.  
   - Upload it to the **"Home_Sales" GitHub repository**.  
