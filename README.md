# DataAnalysis_for_DataEngineeringSalaries2024

This notebook documents an in-depth analysis of the 2024 data engineer salaries dataset obtained from Kaggle. Utilizing Apache Spark within Databricks, the analysis covers data ingestion, transformation, and visualization to derive meaningful insights.

# Objectives for Data Analysis
**1. Dataset Setup and Inspection:**

* Accessed AWS S3 to load the 2024 data engineer salaries dataset.
* Displayed the first 10 records of the dataset.

**2. Table Creation and SQL Queries:**

* Created `salaries_table` in Spark SQL.
* Executed SQL queries to analyze average salary by job title, max salary by experience level, and count employees by company size.

**3. Visualizations:**

* Line chart: Average salary over time.
* Bar charts: Average salary by experience level, remote work ratio by company size, job titles, and top countries.
* Scatter plot: Average salary vs. remote work ratio for top countries.

**4. Data Transformations:**

* Filtered, selected, limited, and ordered the dataset.
* Grouped by job title with aggregation functions.
* Calculated min/max salaries, distinct job titles, and salary-remote ratio correlation.
* Created a widget for country filtering.
* Filled null values in `remote_ratio` with the mean.
* Added `is_full_time` column based on `employment_type`.
* Wrote DataFrame in Delta format and created a temporary view.

**5. Performance Analysis:**

* Disabled adaptive query executor.
* Analyzed number of partitions and optimized query performance.

This analysis leverages the capabilities of Apache Spark for large-scale data processing and aims to provide actionable insights into the salary trends of data engineers in 2024.
