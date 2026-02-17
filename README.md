# Hospitality-Domain-EDA-using-Python
This project explores hotel booking data to understand occupancy patterns, revenue performance, customer behavior, and operational gaps across properties, cities, and room categories. 
The analysis focuses on transforming raw booking records into business insights that can support pricing, capacity planning, and decision-making in the hospitality domain.

Dataset size:

~134k booking records
multiple dimension tables
aggregated operational dataset

# Objective
Analyze booking and occupancy trends across hotels
Identify revenue drivers and utilization gaps
Understand customer booking behavior and cancellation patterns
Detect data quality and operational issues
Provide actionable insights for business improvement

# Dataset Overview

The project uses a star-schema style dataset with dimension and fact tables.

# Dimension tables

dim_date – date, month, week, weekday/weekend classification for trend analysis
dim_hotels – hotel details including city and category (Luxury/Business)
dim_rooms – room categories and classifications

# Fact tables

fact_bookings – transactional booking data including booking status, guests, platform, revenue generated and realized
fact_aggregated_bookings – aggregated occupancy and capacity data for operational analysis

# Tools & Technologies

Python
Pandas
NumPy
Matplotlib
Seaborn

Jupyter Notebook
# Dataset Architecture
This project uses a star-schema style structure.

Dimension tables 

dim_date (92 rows, 4 columns)
Fields:
date
month-year
week number
day type (weekday/weekend)

dim_hotels (25 rows, 4 columns)
Fields:
property_id
property_name
category (Luxury / Business)
city

dim_rooms (4 rows, 2 columns)
Fields:
room_id
room_class (Standard, Elite, Premium, etc.)

Fact tables (transaction data)
fact_bookings (134,590 rows, 12 columns)

Fields include:
booking_id
property_id
booking_date
check_in_date
checkout_date
number_of_guests
room_category
booking_platform
ratings_given
booking_status
revenue_generated
revenue_realized

fact_aggregated_bookings (9,200 rows, 5 columns)
Fields:
property_id
check_in_date
room_category
successful_bookings
capacity


