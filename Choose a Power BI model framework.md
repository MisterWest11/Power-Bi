# Describe Power BI model fundamentals

**Data Model**- it is a query-able data resource that's optimized for analytics. Reports can query data models by using one of two languages: Data Analysis Expressions(DAX) or Multidimensional Expressions(MDX).

**Power BI dataset**- A dataset is a Power BI artifact that's a source of data for visualizations in Power BI reports and dashboards.

**Analytic query**- an analytica query produces a query result from a model that's easy for a person to understand, especially when visualized.
                  it has an 3 phases: Filter, Group and Summarize.

*Filtering*: narrows down the data you see in the report. You can filter by various attributes like time period or product category. Filters are applied at different levels (report, page, visual) and can be hidden (slicers) or visible (RLS).

*Grouping*: organizes data into categories. Each group acts like a filter but the category itself is shown in the results (e.g., grouping by customer).

*Summarization*: condenses data into a single value. This is often done using functions like sum, count, average on numeric fields. You can summarize data simply or create more complex summaries with DAX formulas.

# Tabular Model

It comprises one or more tables of columns. can include relationships, hierarchies and calculations.

# Star schema design

To produce an optimized and easy-to-use tabular model, we recommend you produce a star schema design. It requires you to classify model tables as either dimension or fact.

Dimension tables describe business entities, the things you model. Entities can include products, people etc.

Fact tables store observations or events and can be sales orders, stock balances, exchanges rates... It contains dimension key columns that relate to dimension tables, and numeric measure columns. A fact table forms the center of a star and related dimension tables form the points

![image](https://github.com/MisterWest11/Power-Bi/assets/152319557/a0e12806-fafa-4559-ba4c-bf3b90aa3b61)

# Storage Modes

**Import**: Data is copied and stored within the Power BI model itself. This allows for fast analysis without relying on the original data source.

**DirectQuery**: Queries bypass the model and directly access the original data source. This is useful for very large datasets but can be slower for complex analysis.

**Dual**: A combination of Import and DirectQuery. Power BI can use cached data (Import) when possible or go directly to the source (DirectQuery) for optimal efficiency.

# Model Frameworks

These frameworks define how your entire Power BI model functions based on the storage modes of its tables:

**Import Model**: All tables use the Import storage mode. This is the simplest and fastest option for smaller datasets.

**DirectQuery Model**: All tables use the DirectQuery storage mode. This is suitable for very large datasets but may have performance limitations.

**Composite Model**: A combination of Import and DirectQuery storage modes within different source groups. This offers flexibility for handling data of varying sizes and performance needs.
