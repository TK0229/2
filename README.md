**Bellabeat Plays It Smart - Case Study**

**About the Company**

Bellabeat, is a company that has understood what the consumers want and has delivered those needs. It has become a thriving high-tech company that manufactures health-focused products that collect data on activity, sleep, reproductive health and stress. 

The company has five successful wellness products: Bellabeat App, Leaf, Time, Spring, and Bellabeat membership. The company is now interested in increasing growth and has asked to utilize data to gain insights into how consumers are currently using their smart devices. The findings discovered from data collected will then help guide a marketing strategy for Bellabeat.



**Phase 1: ASK**

**Identify the Business Task**

How can Bellabeat create a marketing strategy that follows smart device usage trends to maximize growth in the market. 

**Two Questions to Analyze from Fitbit Usage Data:**

What are current trends of smart device usage?

How could these trends influence Bellabeat marketing strategy?

**Primary stakeholders:**

→  Urska Srsen, Bellabeat’s co-founder and Chief Creative Officer

→  Sando Mur, Mathematician and Bellabeat’s co-founder.

**Secondary stakeholders** 

→ Bellabeat’s marketing analytics team. 

**PHASE 2: Prepare:**

**FitBit Fitness Tracker Data**

The public dataset used for analysis is available from https://www.kaggle.com/datasets/arashnic/fitbit. It contains 18 CSV files with personal fitness tracking statistics from fitbit users.

**The dataset has some limitations as discussed below:**

→ Sample size is small; approximately 30 users consented compared to the potential global population of users there could be who use wellness      products.

→ Outdated data; data was collected about 7 years ago.

→ Short duration; Data was only collected during 2 months of the year (03.12.2016-05.12.2016).

**However, the dataset has credibility as discussed below:**

→ Consent was obtained; resulting in accurate personal data.

→ Hourly data was collected; providing insights on when products are used.

→ Variety of minute-level data was collected for physical activity, heart rate, and sleep monitoring.

**PHASE 3: Process**

For this analysis, a combination of Microsoft Excel and BigQuery SQL were used. Firstly, Excel is used to clean the data to avoid any duplicates, errors and understand any noticeable trends. 

**Excel**

→ Used ‘duplicate data’ tool to check for duplicates

→ Formatted date data into MM/DD/YY date formats

→ Formatted all numerical data into Number format

→ Used ‘filter’ and ‘count’ to determine how many users there were in each file. 

After cleaning the data, I decided to merge hourly calories, hourly steps and hourly intensity data to its own tab to observe any trends. The following were my observations:

→ Most exercise activity occurred in the early morning hours and the evening hours. 

→ Most users used their devices for the majority of the day, on average 21 hours.

→ Some files contained less than 10 users while some contained 33. The files with less users were then not used for further analysis. 

After cleaning up data, I uploaded the CSV files in BigQuery to analyze the data further.

**PHASE 4: Analyze**

**BigQuery SQL**

First I checked how many times each user used the FitBit tracker. 

<img width="672" alt="Screen Shot 2023-02-10 at 10 51 08 PM" src="https://user-images.githubusercontent.com/125219650/218337623-58b9116b-750d-4753-8a05-5e8084c4f428.png">

