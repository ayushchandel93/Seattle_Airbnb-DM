# Seattle_Airbnb Relational Database Model in 3NF and Physical Database Creation

**Data Source**
_________________________________________________________________________________________________________________________________________________________________________________
- Kaggle: https://www.kaggle.com/airbnb/seattle

**Data Files**
_________________________________________________________________________________________________________________________________________________________________________________
- One listings.csv file that contains Airbnb listing information and Airbnb host information
- One calendar.csv file that contains property availability information throughout the year
- One reviews.csv file that contains Airbnb property reviews information

**Extract**
_________________________________________________________________________________________________________________________________________________________________________________
- CSV files are taken from a Kaggle web page and saved in the "Resources" folder
- Data is extracted from the four CSV files in the "Resources" folder
- Excel is used to extract data from the CSV files is listed below:
1. listings.csv
2. calendar.csv
3. reviews.csv

Idea for Relational Database Schema
Fourteen tables:
One table with hosts information from the listings.csv file
One table of review rating from the reviews.csv file
One table of review from t




or listings information from the listings.csv file
One table with hosts information from the listings.csv file
One table with property availability information from the calendar.csv file
One table with property reviews information from the reviews.csv file


**Relational Data Model**
_________________________________________________________________________________________________________________________________________________________________________________
- **Assumptions/Notes About Data Entities and Relationships**


1.	Airbnb has 1:M relationship with review rating. Each Airbnb can have multiple review ratings.
2.	Host has 1:M relationship with Airbnb. As host can have several Airbnb properties.
3.	Airbnb has 1:M relationship with review. As one Airbnb can have multiple reviewers & reviews.
4.	Airbnb has 1:1 relationship with property type. As each Airbnb can have specific property type.
5.	Host has 1: M relationship with property type. As one host can have several properties with different property types.
6.	Host has 1:M relationship with review. As one host can have many reviews.
7.	Property type has a 1:1 relationship with price. As one property can have a fixed price.
8.	Review has a 1:1 relationship with comments review. As for review ID there is only one comment.
9.	Location has 1:M relationship with Airbnb. As 1 location can have several Airbnb.
10.	Airbnb has 1:M relationship with calendar. As 1 Airbnb can be available on several dates.
11.	Airbnb has 1:1 relationship with property availability. As it tells us maximum and minimum available nights of a specific Airbnb.
12.	Airbnb has 1:1 relationship with Price. As 1 property can have single price.
13.	Location has M:1 relationship with Street. As a single location can have multiple streets in it.
14.	Street has M:1 relationship with Zipcode. There are different zipcode for different streets.
15.	Zipcode has M:1 relationship with City. In a single city there are many zipcodes according to areas.
16.	City has M:1 relationship with State. As one state can have multiple cities.


**Entity-Relationship Diagram**

![image](https://user-images.githubusercontent.com/96445991/147801266-db0ad244-fe15-4f97-893e-3f52e4608205.png)


**Physical MySQL Database**
_________________________________________________________________________________________________________________________________________________________________________________

- **Notes About Data Set**

1.	AirBnb: Contains unique listing ID of each and every AirBnB property.
2.	Host: Identifies details of Airbnb property owners.
3.	Calender: Contains information about available date and price of airbnb’s.
4.	Review_Rating: It stores review related data like dates, score and accuracy
5.	Comments_review: contains reviewers name and there comment
6.	Price: contains price details of the specific property.
7.	Property_availability: contains maximum and minimum nights available details of specific property.
8.	Property_type: Describes property features like no. of bedrooms, baths etc.
9.	Location: Stores information of the neighborhood.
10.	Street: Has all the data of the streets where AirBNB’s are located.
11.	Zipcode: Zipcode of all the address is stored in here.
12.	City: Stored the cities where AirBNB’s are located.
13.	State: Stored the cities where AirBNB’s are located.


**Data in the Database:**
_________________________________________________________________________________________________________________________________________________________________________________

![image](https://user-images.githubusercontent.com/96445991/147801761-a1efa1c8-3fa7-41e2-884b-1be767629f40.png)




**Screen shot of Physical Database objects**
_________________________________________________________________________________________________________________________________________________________________________________

**Screenshots of 10 tables from database along with the data below:**
_________________________________________________________________________________________________________________________________________________________________________________

1. Airbnb

![image](https://user-images.githubusercontent.com/96445991/147801447-cdb00961-191c-4280-95c1-bab466cdd3d8.png)


2. Property Availability

![image](https://user-images.githubusercontent.com/96445991/147801482-1e95c6c0-3baf-4e6d-be6b-cd445218c5e8.png)


3. Location 

![image](https://user-images.githubusercontent.com/96445991/147801492-ead46dcf-5f39-4bbf-a0eb-18865957f63a.png)


4. Host

![image](https://user-images.githubusercontent.com/96445991/147801497-0d56a867-a82a-480f-bcd9-288401c86778.png)


5. Calender

![image](https://user-images.githubusercontent.com/96445991/147801501-8015adf2-d3d7-49ab-96c6-0ee8dec73f97.png)


6. City

![image](https://user-images.githubusercontent.com/96445991/147801518-d821a9b5-334b-493e-9136-d05385f3f667.png)


7. Price

![image](https://user-images.githubusercontent.com/96445991/147801524-ecc1056a-8f5a-4da2-ae9a-99bdbb706c29.png)


8. Property type

![image](https://user-images.githubusercontent.com/96445991/147801526-f837bcae-b883-40e5-bed2-35185b00e88e.png)


9. Review rating

![image](https://user-images.githubusercontent.com/96445991/147801533-01b01a04-e211-446d-9beb-162c8674a6e7.png)

10. State

![image](https://user-images.githubusercontent.com/96445991/147801539-9b20299b-e551-46a9-afe0-cf9ca0bc85c0.png)



