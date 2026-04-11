# Clinical Operations Dashboard

The Clinical Operations Dashboard is a Power BI solution designed to provide a comprehensive overview of clinician and branch performance. It enables stakeholders to monitor operational efficiency, track key performance indicators (KPIs), and quickly identify areas that require improvement or further attention.

The dashboard is built to support data-driven decision-making by transforming raw operational data into meaningful insights. It offers both high-level summaries and detailed breakdowns, allowing users to analyze trends, compare performance across branches, and evaluate clinician activity over time.

A key feature of this dashboard is its interactive design, which allows users to dynamically switch between different KPIs and aggregation levels within each visualization. This flexibility ensures that users can explore the data from multiple perspectives without needing separate reports or views.

Overall, the goal of this project is to improve visibility into clinical operations, enhance performance tracking, and support continuous improvement across all branches.

## Objectives

The primary goal of this project is to build an interactive dashboard that provides both high-level insights and flexible data exploration through dynamic aggregation in each visualization. Additional objectives include:

1. Create a trend chart across a variety of KPIs
2. Compare performance across different branches
3. Analyze the distribution of patient visits using multiple dimensions

## Dashboard Development

The development of this dashboard focused on building a robust summary layer and implementing dynamic calculations using DAX, particularly through SWITCH-based measures. Each main visualization includes a dropdown menu in the top-right corner that allows users to select a KPI or parameter, dynamically changing the aggregation within the chart. This enables a more interactive and flexible view for each graph.

- Data was sourced from CSV files provided by the client. Minimal data cleaning was required, except for the branches dataset, where the first row needed to be promoted as headers.
- `table_creation.jpg` illustrates the DAX used to create a weekly summary table that supports the dashboard’s calculations.
- `table_relationships.jpg` shows the star schema design, highlighting relationships between fact and dimension tables. The measures table is excluded from relationships and is used solely for parameter-driven calculations.
- `switch_measure.jpg` demonstrates the DAX SWITCH measures used to enable dynamic aggregation and interactive metric selection across the dashboard.
- `Dashboard.jpg` displays the completed dashboard, showcasing the final layout, visualizations, and interactive features.
