Bank Marketing Data Cleaning
Cleans and restructures raw bank marketing campaign data into three normalised tables ready for analysis.

Overview
Reads a single CSV file and splits it into three separate datasets — client demographics, campaign activity, and economic indicators — applying type conversions, null handling, and date parsing along the way.
    
Prerequisites
Python 3.8+
pandas
numpy

Usage
Place bank_marketing.csv in the same directory as the script, then run:
bashpython bank_marketing.py

Input
bank_marketing.csv — raw bank marketing data containing client, campaign, and economic columns.
Output

client.csv demographics and financial profile
campaign.csv Campaign contact history and outcomes
economics.csv Economic indicators at time of contact

Data Decisions

education: unknown values treated as missing (NaN)
credit_default, mortgage: unknown mapped to False 
last_contact_date: constructed from separate day, month, and year columns and stored as a datetime
