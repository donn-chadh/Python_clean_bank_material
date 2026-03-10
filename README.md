Cleaning Bank Marketing data:
This project reads in a single dataset and splits it into three clean structured files ready for analysis or storage. 

Client data cleaning
- dots in both job and education columns are replaced with underscores for consistency.
- Unknown values in education are replaced with NaN - mainly to showcase my understanding of Numpy.
  - credit_default and mortgage columns are mapped to boolean to make anaylis easier.
 
Campaign data cleaning
- previous_outcome and campaign_outcome converted to boolean to make analysis easier.
- Created las_contact_data columns to allow filtering during anaylsis
- Dropped redundant columns, month, day, year

Output:
Three CSV files: client.csv, campaign.csv, economics.csv

Tools:
Python, Pandas, Numpy

Author:
Don North
