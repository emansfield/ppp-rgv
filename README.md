# ppp-rgv
An analysis of Paycheck Protection Program loans in the Rio Grande Valley area of Texas using a combination of Excel, R, and Python, performed in partnership with Denise Cathey. The purpose of this analysis is to see where these loans went in comparison to the number of businesses in each ZIP code. This is based on an analysis by Bellingcat. Many thanks to that charity for its open-source projects. Donate here: https://www.bellingcat.com/donate/

## Data sources
Federal PPP data

Census data from its API:
https://www.census.gov/data/developers/data-sets/cbp-nonemp-zbp/zbp-api.html?fbclid=IwAR2ZtKFqaFuWUUxZEwrTTtmhQ48yan5Z58auN0GuA4zh5FKgYxmmhl7ky20


## Steps

Download files for each ZIP code  by changing the URL to contain each ZIP code. Use formula within ZIP-codes-RGV.xlsx to speed up the process of writing the URLs. Download each JSON file. 

Run the Python script to combine the JSON files into one large CSV. Bring the CSV into R to perform a group_by() and summarize() analysis to show the total number of businesses in each ZIP code. Export the smaller dataset as a new CSV. 

Upload the new CSV into Tableau Public to create a simple visualization of the businesses. 
