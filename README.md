# Seattle_Airbnb-DM

**Data Source**
Kaggle: https://www.kaggle.com/airbnb/seattle

**Data Files**
1. One listings.csv file that contains Airbnb listing information and Airbnb host information
2. One calendar.csv file that contains property availability information throughout the year
3. One reviews.csv file that contains Airbnb property reviews information

**Idea for Relational Database Schema**
Four tables:
One table for listings information from the listings.csv file
One table with hosts information from the listings.csv file
One table with property availability information from the calendar.csv file
One table with property reviews information from the reviews.csv file
How the tables are linked together:
Listings and hosts tables linked together by host_id
Listings and property availability tables linked together by listing_id
Listings and property reviews tables linked together by listing_id
