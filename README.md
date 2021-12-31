# Seattle_Airbnb-DM

**Data Source**
- Kaggle: https://www.kaggle.com/airbnb/seattle

**Data Files**
- One listings.csv file that contains Airbnb listing information and Airbnb host information
- One calendar.csv file that contains property availability information throughout the year
- One reviews.csv file that contains Airbnb property reviews information

**Extract**
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

