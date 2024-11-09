# Data Analysis for AtliQ Hotels

## Overview

This project aims to analyze booking and occupancy data for AtliQ Hotels to uncover key insights about room occupancy, revenue trends, and booking patterns across different hotel properties. Using Python, we import, clean, and transform the data from multiple CSV files to enable meaningful insights. This project covers data exploration, data cleaning, data transformation, and insights generation.

## Datasets

The project uses the following datasets:

- [dim_date.csv](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_date.csv): Date dimension data.
- [dim_hotels.csv](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_hotels.csv): Hotel information.
- [dim_rooms.csv](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_rooms.csv): Room details and types.
- [fact_aggregrated_bookings.csv](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/fact_aggregated_bookings.csv): Aggregated booking data.
- [fact_bookings.csv](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/fact_bookings.csv): Detailed booking information.

## Project Structure

The project is structured into several key sections, each covering specific tasks in the data analysis workflow.

### 1. Data Import and Exploration

- Import each dataset and load them into separate DataFrames.
- Perform initial exploration on the bookings data to understand the structure and summary statistics.
- **Exercises**:
  - Find unique property IDs in the aggregated bookings dataset.
  - Calculate total bookings per `property_id`.
  - Identify dates when bookings exceeded capacity.
  - Determine properties with the highest capacity.

### 2. Data Cleaning

- **Invalid Guests**: Records with negative guest values are removed.
- **Outlier Removal in Revenue Generated**: Outliers are identified using a limit of (average + 3*std). In this dataset, revenue values did not exceed this limit, indicating no outliers in revenue.
- **Null Ratings**: As many records have null ratings, we retain them rather than imputing values.
- **Exercises**:
  - Identify and fill null values in the aggregate bookings dataset.
  - Filter records with `successful_bookings` values exceeding room capacity.

### 3. Data Transformation

- **Occupancy Percentage**: Created a new column `occupancy_percentage` calculated as `(successful_bookings / capacity) * 100`.
- Other transformations:
  - Normalization of values.
  - Merging datasets based on common columns.
  - Aggregation of data to generate meaningful insights.

### 4. Insights Generation

Using transformed data, we answer the following business questions:

1. **Average Occupancy Rate by Room Category**: Calculate average occupancy rate per room type (e.g., Standard, Premium, Elite).
2. **Average Occupancy Rate per City**.
3. **Weekday vs. Weekend Occupancy**: Compare occupancy rates across weekdays and weekends.
4. **Monthly Occupancy for June by City**.
5. **Append New Data for August**: Extend the dataset with new bookings data.
6. **Revenue Realized per City**.
7. **Monthly Revenue Trends**.
8. **Revenue per Hotel Type**.
9. **Average Rating per City**.
10. **Booking Platform Revenue Distribution**: Visualized with a pie chart.

## Libraries Used

- `pandas`: For data manipulation and transformation.
- `matplotlib` / `seaborn`: For data visualization.

## Key Insights

- Identified high-occupancy properties and categories with varying demands across cities and days of the week.
- Monthly revenue trends provide insight into peak times for bookings.
- Discrepancies in occupancy rates between weekdays and weekends highlight booking behaviors.
- Visualizations of revenue by city, hotel type, and booking platform aid in understanding the revenue distribution.

