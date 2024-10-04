# Hotel-Booking-Analysis:

# Objective

This Power BI dashboard provides detailed insights into hotel booking performance, including revenue, total bookings, cancellation rates, guest demographics, and more. It helps hotel management and analysts track key performance metrics for weekday and weekend bookings and analyze city-specific performance, customer behavior, and room category preferences.

## Data Sources

The data model consists of the following tables:

fact_bookings: Contains detailed information about individual bookings, including booking status, room type, and revenue generated.

fact_aggregated_bookings: Aggregated data for bookings with summarizations like total bookings, total guests, and revenue.

dim_date: Date dimension for time-based analysis.

dim_hotels: Contains information about the hotels, including hotel names and categories.

dim_room: Contains details about room categories and types.

## Steps to Create the Dashboard

## Data Import and Model Setup:

Import the data from the respective sources (fact and dimension tables).

Create relationships between the tables. For example, connect the fact_bookings and fact_aggregated_bookings with the appropriate dimension tables (dim_date, dim_hotels, and dim_room).

## KPI Tiles:
Total Revenue: Use the fact_aggregated_bookings table to calculate the total revenue.

Total Guests: Sum the number of guests from the fact_aggregated_bookings table.

Cancellation Rate: Calculate the percentage of bookings with a "Cancelled" status from the fact_bookings table.

Total Bookings: Count the number of unique bookings in the fact_bookings table.

## Weekdays vs. Weekends:

Create measures for Weekday Bookings and Weekend Bookings by applying filters based on the day of the week using the dim_date table.

Display separate KPIs for bookings and revenue on weekdays and weekends.

## Cancellation and Occupancy Gauges:

For each gauge, create measures for Cancellation Rate (%) and Occupancy Rate (%).

Use these to visually indicate booking cancellations and room occupancy percentages, with thresholds for performance levels.

## Revenue Contributors by City:

Create a bar chart visual using the dim_hotels table to show the contribution of each city to total revenue.

Include a calculated measure for Revenue Share by City to highlight which cities are the top contributors.

## Category-Wise Booking:

Create a pie chart to display bookings distribution across different room categories (e.g., RT1, RT2, RT3, RT4) using the dim_room table.

## Average Ratings:

Display the average rating of hotels using data from the fact_bookings table, which contains customer feedback and ratings.

## Revenue by Hotel and Room Category:

Use stacked bar charts to break down revenue contributions by hotel and by room category (Luxury, Business, etc.).

## Booking Source Distribution:

Visualize the proportion of bookings made through different sources (e.g., MakeMyTrip, Tripster, Direct Online) in a pie chart.

Use the fact_bookings table, assuming it contains the booking source data.

## Slicers for Interactivity
Add slicers for Hotel Name, Room Category, and City to allow users to filter the dashboard and focus on specific data points.

## Key Insights Delivered
Revenue and Occupancy Trends: Identify which days of the week or cities contribute the most to revenue and have the highest occupancy rates.

Booking Cancellation Rates: Track the percentage of cancellations to identify problematic areas.

Customer Preferences: Understand which room categories are most popular and which hotels attract the most guests.

## Conclusion

This dashboard provides a holistic view of the hotel booking performance across different dimensions. By using this dashboard, hotel management can easily track KPIs, monitor trends, and make data-driven decisions to optimize their business operations.
