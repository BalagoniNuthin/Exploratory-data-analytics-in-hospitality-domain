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
   - **Description**: This file contains detailed booking information for various properties, including dates, room categories,successful bookings and capacity.
   - **Columns**:
     - `room_id`: `property_id`: A unique identifier for each property (e.g., "16558").
     - `check_in_date`: Scheduled check-in date.
     - `room_category`: Room type identifier.
     - 'successful_bookings' : Number of successful bookings.
     - 'capacity' : Capacity of rooms available.

5.[**fact_bookings.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/fact_bookings.csv) :
   - **Total Rows**: 134590
   - **Total Columns**: 12
   - **Description**: This file contains detailed booking information for various properties, including dates, guest counts, and revenue metrics.
   - **Columns**:
     - `booking_id`: Unique identifier for each booking (e.g., "May012216558RT11").
     - `property_id`: Identifier for each property.
     - `booking_date`: Date the booking was made.
     - `check_in_date`: Scheduled check-in date.
     - `checkout_date`: Scheduled check-out date.
     - `no_guests`: Number of guests per booking.
     - `booking_platform`: Platform through which the booking was made (e.g., "direct online", "logtrip").
     - `ratings_given`: Ratings assigned to the booking by guests.
     - `booking_status`: Current status of the booking (e.g., "Checked Out", "Cancelled").
     - `revenue_generated`: Total revenue generated for the booking.
     - `revenue_realized`: Realized revenue from the booking.

6.[**new_data_august.csv**](https://github.com/BalagoniNuthin/Exploratory-data-analytics-in-hospitality-domain/blob/main/Datasets/new_data_august.csv) :
   - **Total Rows**:7
   - **Total Columns**: 13
   - **Description**: This file contains data on room occupancy for various properties, focusing on capacity and occupancy rates for August.
   - **Columns**:
     - `property_id`: Identifier for each property.
     - `property_name`: The name of the hotel (e.g., "Atliq Grands").
     - `category`: The category of the hotel (e.g., "Luxury", "Business").
     - `city`: The city where the hotel is located (e.g., "Delhi").
     - `room_category`: Room type identifier.
     - `room_class`: The class of the room (e.g., "Standard", "Elite", "Premium", "Presidential").
     - `check_in_date`: Scheduled check-in date.
     - `mmm yy`: The month and year combined (e.g., "May 22").
     - `week no`: The week number within the year (e.g., "W 19").
     - `day_type`: Indicates if the day is a `weekday` or `weekend`.
     - 'successful_bookings' : Number of successful bookings.
     - 'capacity' : Capacity of rooms available.
     - 'occ%' : Occupancy percentage.

