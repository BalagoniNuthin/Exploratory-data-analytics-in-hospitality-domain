# Project Data Files
This repository contains the following data files:
1. [**dim_date.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_date.csv) : 
    - **Total Rows**: 93
   - **Total Columns**: 4
   - **Description**: This file serves as a date dimension table, useful for categorizing and analyzing dates.
   - **Columns**:
     - `date`: The specific date in "DD-MMM-YY" format (e.g., "01-May-22").
     - `mmm yy`: The month and year combined (e.g., "May 22").
     - `week no`: The week number within the year (e.g., "W 19").
     - `day_type`: Indicates if the day is a `weekday` or `weekend`.

2. [**dim_hotels.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_hotels.csv) : 
    - **Total Rows**: 26
   - **Total Columns**: 4
   - **Description**: This file contains details about different hotel properties.
   - **Columns**:
     - `property_id`: A unique identifier for each property (e.g., "16558").
     - `property_name`: The name of the hotel (e.g., "Atliq Grands").
     - `category`: The category of the hotel (e.g., "Luxury", "Business").
     - `city`: The city where the hotel is located (e.g., "Delhi").

3. [**dim_rooms.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/dim_rooms.csv) : 
    - **Total Rows**: 5
   - **Total Columns**: 2
   - **Description**: This file provides information about various types of hotel rooms.
   - **Columns**:
     - `room_id`: A unique identifier for each room type (e.g., "RT1").
     - `room_class`: The class of the room (e.g., "Standard", "Elite", "Premium", "Presidential").
    
4.[**fact_aggregated_bookings.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/fact_aggregated_bookings.csv) :
 - **Total Rows**: 9201
   - **Total Columns**: 5
   - **Description**: This file provides information about various types of hotel rooms.
   - **Columns**:
     - `room_id`: A unique identifier for each room type (e.g., "RT1").
     - `room_class`: The class of the room (e.g., "Standard", "Elite", "Premium", "Presidential").

5.[**fact_bookings.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/fact_bookings.csv) :
 - **Total Rows**: 9201
   - **Total Columns**: 5
   - **Description**: This file provides information about various types of hotel rooms.
   - **Columns**:
     - `room_id`: A unique identifier for each room type (e.g., "RT1").
     - `room_class`: The class of the room (e.g., "Standard", "Elite", "Premium", "Presidential").

6.[**new_data_august.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/new_data_august.csv) :
 - **Total Rows**: 9201
   - **Total Columns**: 5
   - **Description**: This file provides information about various types of hotel rooms.
   - **Columns**:
     - `room_id`: A unique identifier for each room type (e.g., "RT1").
     - `room_class`: The class of the room (e.g., "Standard", "Elite", "Premium", "Presidential").
