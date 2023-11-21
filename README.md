# Airline Bookings and Performance Analysis
## Flight Bookings and Sales Performance Analysis 

### 1. Overview:
The Revenue and Net Planning departments provide you with Spain's (fictional) sales and flight data. The dataset includes the performance of all Easter flights in 2019 and in 2023. With the help of your analysis, they want to compare the company’s sales and flight performance this year vs the pre-Corona status. Based on this comparison, they want you to create actionable insights.

#### Objective:
* What can be done with the data in Power BI? Analyze the provided dataset and provide a dashboard for the stakeholders.
* What key figures can be developed from the dataset?
* Identify interesting trends/outliers/developments and derive actionable insights for the stakeholders.

#### Optional Tasks:
* What additional data from other sources could be included to gain meaningful insights?
* The column for the new route identifier had some issues during the data load. Show us a clever way to fill in the missing data.
* Include ad-hoc analytical scripts in R or Python to gain meaningful insights.


Now we understand the business objectives from the stakeholders, let's start to work on the porject.

 ### - Tools: Power BI and Pytho(Pandas)
 ## 1. DATA ACQUISITION
   The data source is from Kaggle. Link to three csv: https://www.kaggle.com/datasets/banuba/flight-bookings
   
 #### Metadata: Table description
 i. Bookings Table: Containing seven(7) columns:
 - BookingCode: A unique code associated with a booking transaction.
 - BookingDate: The date when the booking was made.
 - FlightDate: The scheduled date for the flight associated with the booking.
 - FlightNumber: The unique identifier assigned to a specific flight.
 - BookedSeats: The number of seats booked in the flight for a particular booking.
 - RevenueActualFare: The actual fare revenue generated from the booking.
 - Ancillary Revenue: Additional revenue generated from ancillary services or add-ons associated with the booking.


ii. Flight Info:

- FlightId: A unique identifier assigned to a specific flight.
- OriginDestination: The route or path indicating the origin and destination airports for the flight.
- CustomClusterName: A customized cluster name or label associated with the flight.
- IsNew: A binary indicator (True/False) denoting whether the flight is classified as new.
- Capacity: The maximum number of seats or passengers the flight can accommodate.
- FlightCosts: The overall costs associated with operating the flight, covering various expenses related to its execution.

iii. Sales Details:
- BookingID: A unique identifier assigned to a specific booking transaction.
- Customer Group: The categorization or grouping of customers associated with the booking.
- Sales Group: The categorization or grouping of sales related to the booking.


## 2. DATA EXPLORATION
Data exploration to have an overview of the dataset are done in python. See jupiter notebook here

## 3. DATA CLEANING
Some data cleaning activities such Fill/drop null values, data validation, etc.. See jupiter notebook

## 4. DATA TRANSFORMATION (ETL)
 Data extracted, transformed and loaded into Power BI for modeling and visualiaztion. 


## 5. DATA ANALYSIS
Deriving insights from using visualisations.

## 5.1 Power BI Dashboard



### 5.1.1: Performance Overview




![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/590fc1dc-e541-4ab3-81aa-eceabac9631e)


### Key Insight:

- Exponential Growth in Revenue: Revenue experienced exponential growth, with an approximate increase of 98% from 2019 to 2023.
  
- Year-over-Year (YoY) Flight Bookings: Year-over-year (YoY) flight bookings increased by over 90% between 2019 and 2023. However, the overall number of bookings, 13,000 in 2019 and 26,000 in 2023 appear relatively low in my opinion.


### 5.1.2: Bookings Trends Analysis




![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/40068894-15dd-48a6-a75d-f9929ef8baf5)


### Key Insight:

- For the Customer Group and Sales Group: In both the Customer Group and Sales Group, 80% of total bookings are generated by end customers and web channels, respectively.


### 5.1.3: Route and Destination Analysis





![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/33473c90-0991-435c-9074-861ef304ffe5)




### Key Insights: 

- Capacity Utilization: The overall capacity utilization is 36%, which seems to be on the lower side. When comparing the capacity utilization of 30% in 2019 to 40% in 2023, it becomes evident that flight capacity was underutilized in each year under review.
  
- Non-Performing Routes: Out of over 1,200 total routes, only 20 of them have achieved over 50% flight capacity utilization. This means that just 2% of the total routes performed above the average capacity.



## 6. RECOMMENDATIONS

- It is advisable to maintain sustained growth in all key metrics, such as revenue, profit, and bookings, during the post-COVID-19 period. To achieve this, strategies implemented by various stakeholders and departments should align with these objectives.

- Steps should be taken to address underperforming customer groups (Corporate, OTA, and Travel Agencies) and sales groups (Direct Connect and GDS). For instance, targeted marketing strategies should be developed to increase bookings from these groups. In fact, the top priority should be to increase overall bookings.

- As observed, the current capacity utilization is suboptimal. Operating at less than 50% capacity is highly inadequate, and it is strongly recommended to take immediate measures to rectify this situation.

- There is a need to evaluate nonperforming routes to determine their viability. It is advisable to discontinue unprofitable such as ACE-STR, ACE-HAM, ACE-DUS, and the like and reallocate resources to more lucrative ones.

- A Root Cause Analysis is recommended. Overall, the sales and flight performance do not appear to be impressive. While there might be a significant percentage increase between 2019 and 2023, the absolute figures for total bookings, total revenue, profits, and capacity utilization rate are relatively low. Hence, further investigation into pricing strategies, effective campaigns, customer experience, feedback, competitor analysis, and many other plausible factors is warranted.



---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## Optional Tasks:

- Missing Values in New Route: To address missing data in the new route identifier, we can use conditional logic. If the flight date for the minimum year is 2023, it is considered a new route. Conversely, if the minimum year of the flight date is 2019, it indicates that the flight has been in operation since 2019, classifying it as an old route.

- Additional Data Sources: 
To obtain a comprehensive view of the trend series, we should include complete data sets for 2020, 2021, 2022, and 2023. Relying solely on data from 2019 and 2023 may not reveal whether there is a recurring pattern during Easter periods or if the observed changes are isolated incidents.Regarding Customer Group: It would be valuable to gather demographic information about customers, such as age and gender data, in order to gain insights into the characteristics of customers that influence booking behavior.



- Outliers/Developments:
Potential outliers have been identified in Booked Seats, Fare Revenue, and Ancillary Revenue (please refer to the box plots below). Consequently, further investigation is necessary to address these influential outliers. If significant outliers are detected through an outlier test, adjustments to the dashboard should be made to accommodate them.

#### Box plot of BookedSheats
![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/ebd203a2-bfcc-4950-9b25-fee903e61aef)




#### Box plot of Ancilliary Revenue

![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/9427d294-c951-4003-b5e3-9d2ab50be3ff)














  

















