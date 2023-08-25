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

 
Mainly performed by using following graph and plots  using Matplotlib and Seaborn library :  
* Bar Plot.
* Scatter Plot.
* Pie Chart.
* Line Plot.
* Heatmap.
* Box Plot.  
## **Univariate Analysis:**  
Performed univariate analysis and made the following conclusions:  
 1.) Agent no. 9 has made most number of bookings.  
 2.) Best adr generating rooms H and G. Hotels should increase the no. of room types A and H to maximise revenue.  
 3.) The most popular meal type is BB(Breakfast).  
 4.) Around 61% bookings are for City hotel and 39% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel.  
 5.) The best market segment for bookings is Online TA.  
 6.) July- August are the busiest and most profitable months for both type of hotels.   
 7.) Most of the guests came from european countries, with highest number of guests from Portugal.  
 8.) Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.  
 9.) Their are only 3.91% repeated customers
 10.) Out of all around 27% bookings are cancelled.
 11.) Portugal, United Kingdom, France, Spain are the countries with most customers.


## **Bivariate Analysis :**  
We tried to answer following questions
 1.) Adr of city Hotel is higher than Resort Hotel aound 11.  
 2.) Online TA is best marketing segment to attract customer(59%).  
 3.) 64.2% bookings are done by couples(onlt two adults as guests).  
 4.) More than 90% bookings in non refund catagory are cancelled.  
 5.) ADR decreases with increase in the number of night stay showing how customers will get a better deal for longer stayes.
 6.) For lead time and total night stay their is no such corelation for practical situations (night stay< 50days & lead time < 50days) but for whole dataset it shows a inverse relationship.  
 7.) Friday has highest number of 2 day visit,which can be weekend holidays. 
 ## **Inferences and Conclusion**
 We’ve drawn many inferences from the above analysis. Here’s a summary of a few of them:
1. City hotels(61.13%) receive more guests throughout the year compared to Resort hotels(38.87%).
2.The average ADR for city hotel is more than resort hotel which is around 11.
3. The booking has increased during the three year period, with maximum in 2016 and a little decrease in 2017. Also, The maximum booking are in thr month of July and August the reason behind it can be holiday season in various countries, good weather for vacation, and summer in colleges and schools. Moreover, the least are in the months of January, November and December.
4. With longer night stay the customers usually get better deal hence the ADR decreases with longer stay.
5. Online TA booking are around 60% followed by offline TA/TO (15.89%) and then Direct booking (13.5%). Promotions and offers should be used to increase direct booking.
6. Out of all the hotel bookings, around 80% are done by TA/TO (Travel agents Tour tour operators), hence we shold be focused on this and work toward increasing Direct direct distribution channel (14.86%).
7. Out of all the bookings, 27.49% are being cancelled, hence seeting Non-refundable Rates, Collect deposits, and implement more rigid cancellation policies.
8. The majority of guests are couples, and families prefer both city as well as resort hotels almost equally.
9. In all only 3.91% are repeated guests, Low number of repeated guests. Hotels need to target repeated guests since retaining a customer is way less expensive than gaining a new one.
10. It appears that a disproportionately high number of bookings are from Portugal, probably because the hotel is located in Portugal itself. The second country is the United Kingdom which is approx. 75% behind.
11. Room type H followed by G yield the most average ADR, Meanwhile P and L contribute the least.
12. Out of the meals, BB (Bed & Breakfast) is the most ordered meal, which is around 77.8% hence hotels should put special attention to this.
13. The six best perforing agents have IDs as 9, 240, 14, 250, 7, 241.

## **Challenges**  
(1) A lot of the data were duplicates.  
(2) Incorrect datatype format for the data was present.  
(3) It was challenging to select the best visualization techniques.  
(4) The dataset contained a large number of null values.  
(5) The range of variables was high hence, we used a log scale for easy visualization.  
