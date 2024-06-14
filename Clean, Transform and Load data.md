# Intorduction

Dirty Data Challenges in Power BI

There are several issues that can make data imported into Power BI unprepared for analysis:

Unformatted Columns: Columns containing numerals instead of text descriptions (e.g., Employment Status).
Errors: 

Data with typos, incorrect values, or inconsistencies.

Missing Values (Nulls): Empty data points that can skew results.

Duplicate IDs: Repeated customer IDs that can lead to inaccurate counts.

Unstructured Data: A single column containing multiple data points (e.g., address with all details combined).

These issues lead to inaccurate reports, misleading visuals, and difficulty in data navigation.

Power BI and Power Query to the Rescue

Power BI offers Power Query, a powerful tool for cleaning and preparing data. Clean data provides several advantages:

Accurate Results: Calculations and aggregations based on clean data will be more reliable.

Organized Tables: Users can easily find the information they need.

Simplified Navigation: Removing duplicates makes filtering and slicing data easier.

Improved Readability: Splitting complex columns or combining multiple ones enhances clarity.

Human-Readable Values: Using descriptive terms instead of codes improves understanding.

This course will teach you techniques for:

Fixing inconsistencies, errors, and null values.

Replacing values with user-friendly terms.

Analyzing data profiles to understand column structures.

Transforming data types for proper calculations.

Reshaping tables for better organization.

Combining queries from different sources.

Implementing clear naming conventions for columns and queries.

Using advanced M code editing for complex transformations.

# Shape the initial data

Shaping Initial Data in Power BI

Power Query Editor allows you to clean and transform data imported into Power BI from various sources. This process ensures the data meets your reporting needs.

Scenario:

You loaded sales data from two sources: a CSV file and an ERP system.

The data appears disorganized, with unnecessary information and incorrect formatting.

Shaping Steps:

Identify Column Headers:

Check if the first row contains column names.

If misplaced, use "Use First Row as Headers" or rename headers individually.

Remove Top Rows:

Eliminate blank rows or rows containing irrelevant data.

Use "Remove Rows" > "Remove Top Rows".

Remove Unnecessary Columns:

Analyze each column for its usefulness in reports.

Remove unnecessary columns using "Remove Columns" options.

Unpivot Columns:

Restructure data from a wide format (multiple columns per category) to a tall format (one column per category).

Useful for combining data from multiple columns into a single column.

Pivot Columns:

Organize flat data (lacking structure) into a summarized table.

Use "Transform" > "Pivot Columns" to group and aggregate data.

# Simplify the data structure

After shaping initial data, you can further refine its structure for easier report creation.

Scenario:

Following the previous data shaping steps, you now need to:


Rename queries for clarity.

Replace incorrect values.

Handle null values.

Remove duplicate entries.

Refining Steps:

*Rename Queries:*

Use clear and user-friendly names that reflect the data content.

Right-click the query in the "Queries" pane and select "Rename".

*Replace Values:*

Use the "Replace Values" feature to correct errors or inconsistencies.

Select the column and choose "Replace Values" from the "Transform" tab.

Specify the values to find and replace.

*Replace Null Values:*

Replace null values with a meaningful alternative (e.g., zero for freight amounts).

Use the "Replace Values" feature following the same steps as above.

*Remove Duplicates:*

Eliminate redundant entries within a column to ensure unique values.

Select the column and choose "Remove Duplicates" from the right-click menu.

*Best Practices for Naming:*

Use common terminology within your organization.

Descriptive business terms are preferred.

Replace underscores with spaces.

Maintain consistency with abbreviations, prefixes, and terms like "number" or "ID".

Avoid overly short or unclear abbreviations.

Remove unnecessary prefixes or suffixes from table names.

Consider how replaced values will appear on reports for readability.

By following these steps and best practices, you'll create a well-structured data model that simplifies report development and improves user understanding.

# Evaluate and change column data types

Power BI automatically detects data types when importing tables, but verification is crucial. Incorrect data types can lead to performance issues and hinder analysis.

Scenario:

While cleaning sales data, you need to ensure columns have the correct data types.

Why Data Types Matter:

Prevent calculation errors, hierarchy derivation issues, and improper relationships.

Example: Incorrect "OrderDate" type (Text) prevents calculating "Quantity of Orders YTD".

Restrict date analysis options (e.g., yearly, monthly) if the date field isn't recognized as "Date".

*Verifying and Changing Data Types:*

Best practice: Verify data types in Power Query Editor before loading data.

Changing Data Types:

  * In Power Query Editor:

      * Select the column and choose "Data Type" from the "Transform" tab.

Select the correct data type from the list.

Alternatively, select the data type icon next to the column header.

In Power BI Desktop Report View (not recommended): Use column tools.

Benefits of Correct Data Types:

Enables accurate calculations and proper relationships.

Allows for date hierarchies for year/month/week analysis.

Additional Notes:

Changes to data types are saved as "Changed Type" steps in Power Query Editor.

Use "Close & Apply" to save changes and apply them to the data model.

Combining Queries in Power BI

Power BI's ability to combine queries is crucial for creating a unified data model. This allows you to combine data from various sources into a single table for analysis and reporting.

# Combine multiple table into a single table

*Combining Scenarios:*

Simplify Model Structure: Reduce complexity by merging numerous tables with similar roles.

Consolidate Data: Combine data from multiple tables with relevant columns into a single table.

Create Custom Columns: Utilize columns from different tables to create a new custom column.

*Merging vs. Appending:*

Appending: Add rows from one table to another (like adding rows from two tables with 300 and 100 rows creates a table with 400 rows).

Merging: Combine data from multiple tables based on a common column (similar to SQL JOIN).

Appending Queries - Example:

Imagine creating a contact information report for employees, suppliers, and customers. Data resides in separate tables: HR.Employees, Production.Suppliers, and Sales.Customers.

Steps:

Reformat Tables:

Remove unnecessary columns.

Ensure relevant columns have identical names across tables (ID, Company, Name, Phone).

*Append Queries:*

In Power Query Editor, select "Append Queries" on the Home tab.

Choose "Append Queries as New" to create a new master table.

Select the tables to append from "Available Tables".

Click "OK" to combine all rows into a single table.

Merging Queries - Example:

Consolidate order and order detail information from separate tables (Orders and OrderDetails) into a single table. The common column is "OrderID".

Steps:

Merge Queries:

In Power Query Editor, select "Merge Queries" on the Home tab.

Choose "Merge Queries as New" to create a new table.

Select the tables to merge and the matching column ("OrderID" in this case).

Choose the join type (e.g., Left Outer for all rows from the first table and matching rows from the second).

Click "OK" to view the merged table.

# Profile data in Power BI

Data profiling is crucial for understanding your data's structure and identifying potential issues before creating reports. Power BI offers features to profile data in Power Query Editor.

Why Profile Data?

Understand data structures (relationships between tables and columns).

Identify data anomalies (outliers that deviate from the norm).

Analyze data statistics (e.g., row counts, value distributions, minimum/maximum values).

Data Profiling Steps:

Explore Data Structure:

View the model structure under the "Model" tab in Power BI Desktop.

Find Anomalies and Statistics:

Go to Power Query Editor ("Transform Data").

Use "Column Distribution," "Column Quality," and "Column Profile" features under the "View" tab.

Understanding Data Statistics:

Column Quality:

Shows percentages of valid, erroneous, and empty data. Ideally, you want 100% valid data.

Column Distribution:

Displays the distribution of values within a column.

Shows counts of distinct (all unique values including duplicates and nulls) and unique values (excluding duplicates and nulls).

Column Profile:

Provides detailed statistics for the first 1,000 rows (by default).

Includes:

Row count: verifies successful data import.

Outliers: identifies unusual values.

Empty rows and strings.

Min and Max: smallest and largest values.

Value distribution graph: shows how often distinct values appear.

For numeric columns, also includes:

Number of zeroes and null values.

Average value.

Standard deviation.

Even and odd value counts.

Benefits of Data Profiling:

Helps identify outliers that might require investigation.

Provides a summary of data distribution within columns.

Serves as a starting point for outlier analysis.
