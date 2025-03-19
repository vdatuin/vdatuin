- 👋 Hi, I’m @vdatuin
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

# PySpark Helper Methods for Databricks

This repository contains a collection of PySpark methods designed to simplify and optimize operations within Databricks environments. These methods cover a range of functionalities from data manipulation, querying historical data, optimizing query performance, to managing and handling Delta Lake operations effectively.

## Purpose

The purpose of these helper methods is to provide developers with ready-to-use, tested PySpark code snippets that can enhance productivity and efficiency when working with large datasets in Databricks. They serve as reference implementations for common tasks such as DataFrame transformations, optimizations, and Delta Lake management.

## Methods Overview

### DataFrame Transformations

#### Selection and Projection
- `select_columns(df, *columns)`
- `select_expressions(df, *expressions)`

#### Column Operations
- `cast_column(df, column_name, target_type)`
- `add_literal_column(df, column_name, value)`

#### Filtering and Sorting
- `filter_data(df, condition)`
- `sort_dataframe(df, *columns, ascending=True)`

### Data Joining

#### DataFrame Joins
- `join_dataframes(df1, df2, join_expr, join_type="inner")`
  - Includes examples for all join types such as inner, outer, left, right, semi, and anti joins.

### Handling Missing Data

#### Fill Missing Values
- `fill_missing_values(df, fill_values)`

### Delta Lake Management

#### Time Travel
- `delta_time_travel(spark, table_path, version=None, timestamp=None)`

#### Z-Ordering and Optimization
- `optimize_table(spark, table_path, zorder_by=None)`

#### Data Cleaning and Maintenance
- `vacuum_table(spark, table_path, retention_hours=168)`

### Advanced Delta Lake Features

#### Delta Time Travel
- Methods to access historical snapshots of data for auditing or analysis.

#### Optimize and Vacuum
- Separate methods to compact files and clean up old files in Delta tables.

## Usage Examples

Each method comes with detailed usage examples, showing how to integrate these functions into your data processing workflows in Databricks. Examples include how to perform complex joins, optimize query performance using Z-Ordering, and manage Delta Lake tables effectively.

## Contributing

Contributions are welcome! If you have improvements or additional helper methods, please submit a pull request or open an issue.


<!---
vdatuin/vdatuin is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
