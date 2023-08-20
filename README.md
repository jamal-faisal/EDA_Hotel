# *Hotel Booking: Exploratory Data Analysis*
## **Objective**
We are provided with a hotel booking dataset.
Our main objective is to perform EDA on the given dataset and draw useful conclusions about general trends in hotel bookings and how factors governing hotel bookings interact with each other.
## **Dataset**
We are given a hotel booking dataset. This dataset contains booking information for a city hotel and a resort hotel. It contains the following features:  
- hotel: Name of hotel ( City or Resort)
- is_canceled: Whether the booking is canceled or not (0 for no canceled and 1 for canceled)
- lead_time: time (in days) between booking transaction and actual arrival.
- arrival_date_year: Year of arrival
- arrival_date_month: month of arrival
- arrival_date_week_number: week number of arrival date.
- arrival_date_day_of_month: Day of month of arrival date
- stays_in_weekend_nights: No. of weekend nights spent in a hotel
- stays_in_week_nights: No. of weeknights spent in a hotel
- adults: No. of adults in single booking record.
- children: No. of children in single booking record.
- babies: No. of babies in single booking record. 
- meal: Type of meal chosen 
- country: Country of origin of customers (as mentioned by them)
- market_segment: What segment via booking was made and for what purpose.
- distribution_channel: Via which medium booking was made.
- is_repeated_guest: Whether the customer has made any booking before(0 for No and 1 for 
                     Yes)
- previous_cancellations: No. of previous canceled bookings.
- previous_bookings_not_canceled: No. of previous non-canceled bookings.
- reserved_room_type: Room type reserved by a customer.
- assigned_room_type: Room type assigned to the customer.
- booking_changes: No. of booking changes done by customers
- deposit_type: Type of deposit at the time of making a booking (No deposit/ Refundable/ No refund)
- agent: Id of agent for booking
- company: Id of the company making a booking
- days_in_waiting_list: No. of days on waiting list.
- customer_type: Type of customer(Transient, Group, etc.)
- adr: Average Daily rate.
- required_car_parking_spaces: No. of car parking asked in booking
- total_of_special_requests: total no. of special request.
- reservation_status: Whether a customer has checked out or canceled,or not showed 
- reservation_status_date: Date of making reservation status.
Total number of rows in data: 119390
Total number of columns: 32
## **Data Cleaning and Feature Engineering**
### (1) Removing Duplicate rows
All duplicate rows were dropped.
### (2) Handling null values
Null values in columns agent were replaced by 0.
Dropped the column company as it has little to no significance in insights.
Null values in column country were replaced by 'others'.
Null values in column children were dropped as only 4 rows had null.
### (3) Converting columns to appropriate data types
Changed data type of children, company, agent to int type.
Changed data type of arrival_date to date type.
### (4) Removing outliers
One outlier was found in the adr column. Simply dropped it while creating the plot.
### (5) Creating new columns
Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.
Created new column arrival_date by adding arrival_date_year+arrival_date_month+arrival_date_day_of_month.
Created new column arrival_day of arrival_date .
## **Exploratory Data Analysis**
Performed EDA and tried answering the following questions:   
 Q1) Correlation between the variables of the dataset.   
 Q2) Which type of Hotel is mostly booked ?   
 Q3) Which type of Hotel have more avegare ADR?  
 Q4) Time wise analysis of hotel booking over years, months, and days.  
 Q5) Which category visit most in specific months?  
 Q6) Which market segment attract more customers?  
 Q7) Market Segment according to Hotel type ?  
 Q8) Which distribution channel is used most by customers?  
 Q9) Distribution channel according to hotel type? What are the average revenue collection in each month ?  
 Q10) What are the days of the week mostly visited ?   
 Q11) How many of the customers are hotels able to retain?  
 Q12) Hotel booking and choice of hotel type by guests catagories?  
 Q13) Total booking canceled and the booking canceled analysis based on deposite type?   
 Q14) What is the relationship between total night stay with ADR and lead time?  
 Q15) Which country have the biggest customer share?  
 Q16) How many customers are from Europe? Which type of room is mostly demanded ?  
 Q17) Country wise analysis of ADR.  
 Q18) Which type of room give highest revenue ?  
 Q19) How many nights stay will accounts for maximum revenue?  
 Q20) Which meal type is the  most preferred meal of customers?  
 Q21) Which agent has booked the most hotel and generate more revenue?

 
Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:  
* Bar Plot.
* Scatter Plot.
* Pie Chart.
* Line Plot.
* Heatmap.
* Box Plot.

 
