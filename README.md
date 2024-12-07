# Home_Sales

# Home Sales Analysis

This repository contains a PySpark project to analyze home sales data using SQL queries. The goal is to extract insights from the dataset, optimize query performance, and perform data partitioning for efficient querying.

## Getting Started

### Prerequisites
	•	Install PySpark in your environment.
	•	Ensure Python is installed on your system.

### Files
	•	Home_Sales.ipynb: Jupyter Notebook containing the PySpark code for analyzing the dataset.
	•	home_sales_revised.csv: Dataset used for this project.

## Dataset

The dataset includes information about home sales, such as the number of bedrooms, bathrooms, date built, square footage, and price. The home_sales_revised.csv file is the input data for this project.

## Instructions
	1.	Rename the Home_Sales_starter_code.ipynb file to Home_Sales.ipynb.
	2.	Import the necessary PySpark SQL functions in the notebook.
	3.	Load the home_sales_revised.csv dataset into a Spark DataFrame.
	4.	Create a temporary table called home_sales for SQL querying.
	5.	Perform the following tasks using SparkSQL:
### Analysis Tasks:
	 • Calculate the average price for a four-bedroom house sold for each year (rounded to two decimal places).
	 • Find the average price of homes built in each year with three bedrooms and three bathrooms (rounded to two decimal places).
	 • Calculate the average price of homes built in each year with:
	 • Three bedrooms.
	 • Three bathrooms.
	 • Two floors.
	 • At least 2,000 square feet.
	 • (Round off to two decimal places.)
	 • Determine the average price of a home per “view” rating for homes with an average price greater than or equal to $350,000. Log the query runtime (rounded to two decimal places).
	6.	Cache the home_sales temporary table and:
	 • Verify if the table is cached.
	 • Re-run the last query using the cached data and compare the runtime to the uncached runtime.
	7.	Partition the formatted Parquet home sales data by the date_built field.
	8.	Create a temporary table for the partitioned Parquet data and re-run the last query. Compare the runtime to the uncached runtime.
	9.	Uncache the home_sales table and verify that it has been uncached.
	10.	Save and upload the completed Home_Sales.ipynb file to your “Home_Sales” GitHub repository.

## Conclusion

This project demonstrates the power and flexibility of PySpark in analyzing large datasets using SQL queries. By leveraging Spark’s SQL and DataFrame APIs, we efficiently explored the home_sales_revised.csv dataset to extract key insights about home prices based on various features such as bedrooms, bathrooms, size, and view ratings. Additionally, through caching and partitioning techniques, we optimized query performance and showcased the benefits of distributed data processing.

The findings and methodologies here provide a strong foundation for scalable data analysis workflows, making this approach valuable for real-world applications in real estate and beyond.
