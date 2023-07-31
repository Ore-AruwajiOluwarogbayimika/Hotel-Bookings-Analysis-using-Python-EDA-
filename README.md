# Hotel-Bookings-Analysis-using-Python-EDA-
## OVERVIEW 
An indepth analysis using Exploratory Data Analysis (EDA) techniques in python to answer key questions based on the hotel bookings dataset, trends and analysis.

![istockphoto-472899538-612x612](https://github.com/Ore-AruwajiOluwarogbayimika/Hotel-Bookings-Analysis-using-Python-EDA-/assets/129456640/667690ba-3e12-4cb1-bbca-ad2bb6396337)

## OBJECTIVE
The main objective of this project is to carry out Exploratory data analysis using python programming on the hotel bookings dataset and draw useful insights based on the trends, relationships and the connection between the different hotels booked by guests.

## DATA-SET PREVIEW 
The dataset provided (hotel bookings dataset) provides data concerning two (2) different hotels; Resort Hotels and City Hotels. The dataset contains the following columns:

DATASET: Total Rows: 119390
         Total Columns: 32
         
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


## STEPS IN ANALYSIS (ASK, PREPARE, PROCESS, ANALYZE, SHARE, ACT)

1. ### ASK PHASE
   This phase includes pointing out the key objective of the project to aid better focus and results which is: To carry out Exploratory data analysis using python programming on the hotel bookings dataset and draw useful insights based on the trends, relationships and the connection between the different hotels booked by guests.

2. ### PREPARE PHASE
   In this phase, the excel file (Hotel bookings) is downloaded on my local desktop and stored before further analysis.

3. ### PROCESS PHASE
   To begin this phase, the excel file is opened in jupyter notebook for analysis using python programming language. Before analysis, the dataframe in jupyter notebook needs to be cleaned to ensure accurate results.
   
   The data cleaning process involves the following stages:
a. Removing duplicate rows: All duplicate rows were dropped.
b. Handle missing or null values: Null values in "company" and "agent" columns were replaced by 0.
Null values in "country" column were replaced by 'others'.
Null values in "children" column were replaced by the mean of the column.
c. Convert columns to appropraite datatypes: Changed data type of children, company, agent to int type.
d. Adding imporatant columns necessary for analysis: Created new column total_stay by adding stays_in_weekend_nights+stays_in_week_nights.
Created new column total_people by adding adults+children+babies.
e. Removal of Outliers: An outlier in the adr column was dropped.


4. ### ANALYZE PHASE
   In this phase, Exploratory Data Analysis (EDA) was used in analyzing the dataframe and drawing out valuable insights. For this analysis, 10 key questions were answered as regards the objective of the project. The 10 questions are:

 Question 1)  Which room type is the most in demand?
 
 Question 2)  Which room type generates the  highest adr (average daily rate)?
 
 Question 3)  Which meal type is the most preffered meal of customers?
 
 Question 4)  What is the  percentage of bookings in each hotel?
 
 Question 5)  Which is the most common channel for booking hotels?
 
 Question 6)  Which are the top 10 most busy months?
 
 Question 7)  From which country do we have most guests?
 
 Question 8)  How long do people stay at the hotels?
 
 Question 9)  Which hotel seems to make more revenue?
 
 Question 10) Which hotel has a higher chance of repeated stay?

Alongside the code and analysis were visualizations for each question to provide clear insights towards the answers of each question.


6. ### SHARE AND ACT PHASE
The answers provided through the analysis put forth some valuable insights, recommendations and conclusions;

## KEY INSIGHTS

 1.) Most demanded room type is A. but better adr generating rooms H, G and C. Hotels should increase the no. of room types A and H to maximise revenue.
 
 2.) The adr generating rooms are: H, G and C. With room H having the highest Average Daily Revenue. 
 
 3.) Most popular meal type is BB(Bed and Breakfast).
 
 4.) Around 60% bookings are for City hotel and 40% bookings are for Resort hotel, therefore City Hotel is busier than Resort hotel.
 
 5.) The most preferred channel for booking is the TA/TO channel. Guests also use other channels.
 
 6.) August is the busiest and most profitable month for both hotels. This is an idication that guests love booking during the summer holidays.
 
 7.) Most of the guests came from european countries, with highest number of guests from Portugal.
 
 8.) Most common stay length is less than 4 days and generally people prefer City hotel for short stay, but for long stays, Resort Hotel is preferred.
 
 9.) City Hotels make more revenue than Resort Hotels.
 
 10.) Resort Hotel has a higher chance of repeated stay than the city hotels.


 ## RECOMMENDATIONS
 1. Couples are the most common guests for hotels, hence, hotels can plan packages that match couples interest to increase revenue.
 2. Most of the guests came from european countries, with most of guests coming from Portugal, hence, the hotel management can promote various events in portugal to increase the inflow of guests from the country and other top countries.
 3. Since guests prefer to use TA/TO channel for hotel bookings, this can be a focal point for advertisement and marketing, to reach more customers and promote more deals to incoming guests.
