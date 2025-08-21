# Your Task  
**CSV:** https://docs.google.com/spreadsheets/d/106VMqDhav1rPpEhVJHYQqEW8yZ_kxml7/edit?usp=sharing&ouid=110539250374045439410&rtpof=true&sd=true

# Responses 
https://docs.google.com/document/d/1ZrNS7AdxQCT9MbgPhDBhdLkGijLVOiOK8G1Tw4h_8b4/edit?usp=sharing

# Data 
Upload the original data set into the link in pd.read_csv

**Overview of Task**
I was assigned to look at traffic data of AeroConnect between cities in Australia to Foreign Ports. 

**Process**
- Cleaned the data so that the first column contained both the year and the month, then got rid of those specific columns (reduce redundancy). 
- Renamed Month column to Date for clarity 

- When looking at most trafficked Routes, went about this a couple different ways. 
   - First looked at only passenger traffic on a specific month/year. 
   - Then combined passenger traffic with mail and freight weight (Converted passenger traffic to tons as well to be consistent)
      - About 10 routes that had no traffic (most probably missing data)
   - Grouped by city pairs and added up the Passenger Total there. 

- Drew Insights on most traveled years, most traveled routes, passengers in vs passengers out 

# Model 
- Used a Random Forest Model as this was non linear graph 
- Features involed lag of 12 months so that it uses historic data to look at spikes and drops 