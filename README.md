# Blinkit_dataset_analysis
https://docs.google.com/spreadsheets/d/1lBkCkjkszk9gL93V16KMXX06Yox44YmAJ7ormyYYUPA/edit?usp=sharing

# Looker Studio Link
https://lookerstudio.google.com/reporting/812bcbe2-3de6-4e8f-ac81-69e58314562e
# **Project overview**
The Blinkit Dataset here shows delivery performance across orders, highlighting on-time rate, delay distribution, delivery time versus distance patterns, and top delay reasons. It tracks trends by date and identifies outliers and partners driving delays to guide operational improvements. It also has insights about the stock that is recieved in the warehouses and whether it is damaged or correct along with the quantity and price of the items.

<img width="1920" height="1081" alt="image" src="https://github.com/user-attachments/assets/82598029-c0af-491e-9440-dea011923787" />

# File Details 

File Name: Blinkit Dataset

# Data Dictionary
| Column Name            | Description                                                                 | Data Type    |
|------------------------|-----------------------------------------------------------------------------|-------------|
| order_id               | Unique numeric identifier assigned to each order.                          | Integer     |
| delivery_partner_id    | Unique identifier for the delivery partner handling the order.             | Integer     |
| promised_date          | Date on which the delivery was promised to the customer (YYYY-MM-DD).      | Date        |
| promised_time          | Time at which the delivery was promised (HH:MM:SS).                        | Time        |
| actual_date            | Actual delivery date (YYYY-MM-DD).                                         | Date        |
| actual_time            | Actual delivery time (HH:MM:SS).                                            | Time        |
| delivery_time_minutes  | Difference between actual and promised delivery time in minutes.           | Integer     |
| distance_km            | Distance between pickup and delivery location in kilometers.               | Float       |
| distance_bucket        | Categorized delivery distance (e.g., 0-2 Km, 2-4 Km).                      | Categorical |
| delivery_status        | Delivery performance category (On Time, Slightly Delayed, Significantly Delayed). | Categorical |
| reasons_if_delayed     | Operational reason recorded for delay (e.g., Traffic). May be blank.       | String      |
| Final_reason           | Final standardized reason for delay (e.g., Traffic, No Reason).            | Categorical |
