# British Airways Flight Operations Analysis Using PostgreSQL
# By Ofolebe Cyndi
---

![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/british_airways_image.png)

---
## INTRODUCTION

British Airways operates a large network of flights, with different aircraft, routes, and passenger patterns to manage.
This project explores British Airways flight data to understand areas such as aircraft efficiency, passenger trends, cancellations, popular destinations, and additional revenue opportunities.

The aim of this analysis is to uncover patterns within the data and highlight insights that can help better understand flight operations and customer demand.

## PROBLEM STATEMENT

British Airways generates a large amount of flight data, but raw data alone does not explain how different operational factors affect performance.

This project focuses on exploring key questions around flight demand, aircraft usage, cancellations, passenger trends, and revenue opportunities to uncover patterns that provide a clearer understanding of the business.

## BUSINESS QUESTIONS

This analysis was guided by the following questions:

1. Which aircraft manufacturers and models are most commonly used?

2. Which aircraft models demonstrate better fuel efficiency?

3. Which routes and destinations have the highest passenger demand?

4. What trends can be identified in flight cancellations?

5. How does passenger activity change over time?

6. How much additional revenue is generated from services such as baggage fees?

## DATA OVERVIEW 

The dataset used for this project contains British Airways flight information, including details on flights, routes, aircraft, passengers, and operational activities.

## TOOLS USED

- Excel — Data cleaning and preparation before database analysis
- PostgreSQL — Database creation, data management, and SQL-based analysis

## SKILLS DEMONSTRATED

- Data cleaning and preparation
- Relational database creation and management
- SQL querying and data analysis
- Translating business questions into analytical queries
- Identifying trends and patterns from data

  ## DATA PREPARATION

Before importing the data into PostgreSQL, the datasets were cleaned and prepared using Microsoft Excel.

The preparation process involved:

- Removing duplicate records.
- Reviewing missing values and handling blanks where necessary.
- Formatting data types to match the requirements of the PostgreSQL tables.
- Standardising date, time, and currency formats.

The cleaned datasets were then imported into PostgreSQL, where relational tables were created for further analysis.


 ## DATABASE DESIGN & DATA MODELLING
This project involved creating a relational database structure in PostgreSQL to organise British Airways flight data for analysis.

The cleaned datasets were transformed into related tables, with each table representing a key area of the business:

- **Aircrafts** — Contains aircraft details and manufacturer information.
- **Flights** — Contains flight-level information, including passengers, routes, status, and revenue-related data.
- **Routes** — Contains information about flight origins and destinations.
- **Fuel Efficiency** — Contains aircraft performance data related to fuel usage.

## Table Creation

The prepared datasets were imported into PostgreSQL, and tables were created with appropriate columns and data types to match the structure required for analysis.

 ## AIRCRAFTS TABLE
  ### Query
  
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/aircrafts_table_code.png)

  ### Result
  
  ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/aircrafts_table2.png)

  ## FLIGHT TABLE
 ### Query
  
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/flight_table_%20code.png)

   ### Result
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/flight_table.png)

   ## FUEL EFFICIENCY TABLE
   ### Query
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/fuel_efficiency_table_code.png)
   
   ### Result
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/fuel_efficiency_table.png)

   ## ROUTE TABLE
   ### Query
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/route_table_code.png)

   ### Result
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/route_table.png)

   ## Entity Relationship Diagram (ERD)

![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/ERD.png)

   
  # ANALYSIS AND VISUALISATION 
  
 ## Which aircraft manufacturers demonstrate higher fuel efficiency?
 ### Query
    
  ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/best_aircraft_via_fuel_effiency.png)

  ### Result 
  
  ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_1.png)

  ### Insight

Among the manufacturers analysed, Mitsubishi recorded the highest average fuel efficiency value in the dataset.

 ## Are British Airways' frequently used aircraft from more fuel-efficient manufacturers?
  
 ### Query
    
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/aircraft_used_more_frequently.png)

 ### Result
   
   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_2.png)

 ### Insight

British Airways uses Boeing aircraft more frequently, although Airbus aircraft showed better fuel efficiency in the dataset.

## Which months recorded the highest number of cancelled flights?

   ### Query

   ![image alt](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/most_cancelled_flights.png)
    
  ### Result
  
   ![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_3.png)
 
 ### Insight

April recorded the highest number of cancelled flights among the months analysed.
Which city  did passengers travel the most?

## Which destinations recorded the highest passenger demand?
### Query

![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/city_most_travelled.png)

### Result 

![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_4.png)

### Insight

London recorded the highest passenger volume in the dataset, making it the most travelled destination among the routes analysed.

 ## How much revenue was generated from baggage services?

 ### Query
 
![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/baggage_overtime_revenue.png)

 ### Result
 
 ![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_5.png)

### Insight

Baggage fees generated over $34 million in additional revenue for British Airways.


## What is the average number of passengers for each month like?
---

### Query

![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/avg_monthly_revenue.png)

### Result

![](https://github.com/Cyndi-24/British-Airways-Analysis/blob/main/BA%20flights%20SQL%20PROJECTS/capstone_images/answer_6.png)

### Insight

January had the highest average number of passengers with an average of 117 passengers per flight.

# Recommendations

Based on the analysis, British Airways can consider the following actions:

- **Prioritise high-demand destinations:** Passenger volume analysis showed that some destinations attract significantly more travellers than others. British Airways can focus scheduling and available resources on these high-demand routes to better serve passenger needs.

- **Improve cancellation management:** Since certain months recorded higher cancellation levels, British Airways can strengthen planning during these periods by improving scheduling decisions and operational preparation to reduce disruptions.

- **Use passenger trends to support planning decisions:** Monthly passenger patterns can help British Airways better prepare for periods of higher demand by aligning flight availability and resources with expected passenger activity.

- **Maximise additional service opportunities:** The revenue generated from baggage services shows the value of additional offerings beyond ticket sales. British Airways can continue improving and promoting relevant services that provide additional value to passengers.

# CONCLUSION

The analysis revealed key patterns in British Airways’ operations, including differences in aircraft performance, passenger demand across destinations, cancellation trends, and the contribution of additional services to revenue.

These findings show how operational data can help identify areas of strength and opportunities for improvement. By understanding where demand is highest, where challenges occur, and which services contribute additional value, British Airways can make more informed decisions to improve efficiency and passenger experience.
