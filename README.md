# STQD 6324 - Data Management
![image](https://github.com/radzmi/STQD6324_Data_Management_Assignment2/assets/152348714/97f1b503-f429-454a-9bdf-9866ab1b91b4)


This repository comprises three distinct components:

1. Jupyter Notebook (.ipynb) Files: These files contain all the code for data analysis and visualization.

2. CSV Files: These are the exported data files from Hive.

3. Screenshots (SS) Folder: This folder contains screenshots that document the steps taken in Hive.

This analysis are performed using Hive. 

## Uploading data into Hadoop
The dataset are very large to be uploaded into hadoop using manual upload method. Alternative method are very crucial in this analysis. First, the dataset are uploded into putty using pscp technique. Then the dataset are pushed into hadoop at specified location. 

## Hive
The dataset then been imported into Hive. For this analysis, I seperated the data into mulitple .csv file as it make it easier to answer each question seperately. Each script are kept in SS folder as screenshot.

## Python
After downloaded all .csv file, the analysis continued to answer all the question and make visualization for each answer. 

## Insights
###Optimal Time for Minimizing Flight Delay:
1. Time of Day:
Morning (10:00 - 12:00): Lowest average delays (under 5 minutes).
Afternoon (13:00 - 17:00): Gradual increase in delays (around 10 minutes).
Evening (20:00 onwards): Significant spike in delays, highest at 23:00 (over 35 minutes).
Best Time to Fly: Early morning.

2. Day of the Week:
Monday: Highest delays (above 10 minutes).
Tuesday: Reduced delays (about 8 minutes).
Wednesday: Slight increase (around 9 minutes).
Thursday and Friday: High delays (just over 10 minutes).
Sunday: High delays (around 8 minutes).
Saturday: Lowest delays, best day for punctual flights.

3. Month of the Year:
January: High delays (above 10 minutes) due to holiday season.
February and March: Improvement in delays (8 and 6 minutes, respectively).
April and May: Further decrease in delays (around 5 minutes).
June, July, August: High delays (over 14 minutes in June, around 13 minutes in July and August) due to vacation travel.
September: Lowest average delay (around 4 minutes).
October and November: Increase in delays (6 and 8 minutes, respectively).
December: High delays (above 10 minutes) due to holiday travel.

4. Best Months for Flights:
April, May, and September: Consistently lower average delays.
September: Best month for punctuality with the lowest average delay (around 4 minutes).

### Factors contributing to flight delays
1. Carrier Delays:
- Average: 2.5 minutes.
- Causes: Maintenance problems, crew availability, baggage handling, operational inefficiencies.

2. Weather Delays:
- Average: 0.5 minutes.
- Causes: Thunderstorms, snow, fog, high winds.

3. National Airspace System (NAS) Delays:
- Average: 3.5 minutes (highest delay).
- Causes: Air traffic control (ATC) restrictions, airspace congestion, airport operations, systemic issues.

4. Late Aircraft Delays:
- Average: 3.3 minutes.
- Causes: Previous flight arriving late, causing a ripple effect on subsequent flights.

5. Security Delays:
- Average: 0.1 minutes (lowest delay).

### Factors Leading to Flight Cancellations:
1. Carrier-Related Issues ("A"):
- Cancellations: Nearly 60,000.
- Causes: Maintenance problems, crew unavailability, operational inefficiencies.

2. Weather-Related Issues ("B"):
- Cancellations: Around 45,000.
- Causes: Adverse weather conditions.

3. National Airspace System (NAS) Issues ("C"):
- Cancellations: Approximately 30,000.
- Causes: Air traffic control restrictions, airport congestion, systemic factors.

4. Security-Related Issues ("D"):
- Cancellations: Minimal impact compared to other categories.

### Flight experiences with the most significant delays and cancellations
1. Positive Correlation:
- Flights with higher delays often have higher cancellations.
- Delays are a significant precursor to cancellations due to cascading operational issues.

2. Outliers in Cancellations:
- Top 5 flights with the most cancellations: Flight numbers 151, 61, 33, 540, and 64.
- These flights have exceptionally high cancellations, indicating severe or persistent issues.

3. Outliers in Delays:
- Top 5 flights with the most delays: Flight numbers 1138, 579, 647, 438, and 268.
- These flights face consistent operational challenges but manage to avoid cancellations more effectively than others.

4. General Trend:
- Most flights experience fewer than 20,000 delays and fewer than 40 cancellations.
- Indicates that while delays are common, cancellations are less frequent for most flights.





















