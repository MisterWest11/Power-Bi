# Star Schema Design

Star schema design is a way to organize data in a data warehouse for easy analysis. It uses two types of tables: fact tables which store the measures or metrics and dimension tables which describes the facts.

**Fact Tables**

The role of a fact table is to store an accumulation of rows that represent observation or events that record a specific business activity.

Fact Table: Store actual data points or events like sales, orders, stock movements etc. they accumulate data over time and are used for calculations in analysis.

Dimension Tables: describe the factual data like products, customers, dates etc. they have unique identifiers additional descriptive columns used for filtering and grouping data.

![image](https://github.com/MisterWest11/Power-Bi/assets/152319557/56c882df-e437-4034-8c54-8c40c1ddbf59)

**Relate Star Schema Tables**

In the model, dimension tables are related to fact tables by using one-to-many relationships. The relationships allow filters and groups that are applied to dimension table columns to propagate to fact table.

Dimension tables can be used to filter multiple fact tables and fact tables can be filtered by multiple dimension table.

![image](https://github.com/MisterWest11/Power-Bi/assets/152319557/2c1c8761-4c06-4b01-ad7d-6fdceb4268f4)

# Analytic Queries

* An analytical query retrieves data based on filters, groups it, and summarizes the results.

* Filters narrow down the data to what's relevant.

* Grouping organizes the data into categories.

* Summarization calculates a single value (sum, count) based on groupings.

an analytical query has three phases that are implemented in this order:

  1. Filter - targets data of revelance.

  2. Group - divides query results into groups.

  3. Summarize - produces a single value result.

# Configure report visuals

Authors add visuals (like charts) and other elements (text boxes, buttons) to report pages.

Visuals are linked to data in the semantic model by mapping fields to specific parts of the visual (e.g., Y-axis, X-axis in a chart).

Mapped fields can be renamed, summarized (calculate total, count etc.) and formatted (change colors, add labels etc.).

