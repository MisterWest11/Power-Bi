# Describe Power BI model fundamentals

**Data Model**- it is a query-able data resource that's optimized for analytics. Reports can query data models by using one of two languages: Data Analysis Expressions(DAX) or Multidimensional Expressions(MDX).

**Power BI dataset**- A dataset is a Power BI artifact that's a source of data for visualizations in Power BI reports and dashboards.

**Analytic query**- an analytica query produces a query result from a model that's easy for a person to understand, especially when visualized.
                  it has an 3 phases: Filter, Group and Summarize.

*Filtering*: narrows down the data you see in the report. You can filter by various attributes like time period or product category. Filters are applied at different levels (report, page, visual) and can be hidden (slicers) or visible (RLS).

*Grouping*: organizes data into categories. Each group acts like a filter but the category itself is shown in the results (e.g., grouping by customer).

*Summarization*: condenses data into a single value. This is often done using functions like sum, count, average on numeric fields. You can summarize data simply or create more complex summaries with DAX formulas.
