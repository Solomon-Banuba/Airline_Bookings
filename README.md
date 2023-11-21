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
 ## 1. DATA ACQUISITION
   The data source is from Kaggle. Link to three csv: ![image](https://github.com/Solomon-Banuba/Airline_Bookings/assets/101892794/ab33568d-ec78-4c17-a131-4966d1099cc8)
   
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

