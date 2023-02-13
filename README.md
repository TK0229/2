# **Bellabeat Plays It Smart - Case Study**

## **About the Company**

Bellabeat, is a company that has understood what the consumers want and has delivered those needs. It has become a thriving high-tech company that manufactures health-focused products that collect data on activity, sleep, reproductive health and stress. 

The company has five successful wellness products: Bellabeat App, Leaf, Time, Spring, and Bellabeat membership. The company is now interested in increasing growth and has asked to utilize data to gain insights into how consumers are currently using their smart devices. The findings discovered from data collected will then help guide a marketing strategy for Bellabeat.



## **PHASE 1: ASK**

**Identify the Business Task:**

How can Bellabeat create a marketing strategy that follows smart device usage trends to maximize growth in the market. 

**Two Questions to Analyze from Fitbit Usage Data:**

What are current trends of smart device usage?

How could these trends influence Bellabeat marketing strategy?

**Primary stakeholders:**

→  Urska Srsen, Bellabeat’s co-founder and Chief Creative Officer

→  Sando Mur, Mathematician and Bellabeat’s co-founder.

**Secondary stakeholders:** 

→ Bellabeat’s marketing analytics team. 

## **PHASE 2: Prepare**

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

## **PHASE 3: Process**

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

## **PHASE 4: Analyze**

**BigQuery SQL**

First, I checked how many times each user used the FitBit tracker. 

<img width="672" alt="Screen Shot 2023-02-10 at 10 51 08 PM" src="https://user-images.githubusercontent.com/125219650/218337623-58b9116b-750d-4753-8a05-5e8084c4f428.png">

The results showed that the majority of users were active users, wearing their tracker anywhere from 25-31 times during the recorded period. There were also some light users; who wore their tracker anywhere from 4 - 14 times. 

Next, I checked how active the users are by closely looking at the AVG of total steps, total calories, total activity level per Id. 

<img width="561" alt="Screen Shot 2023-02-10 at 11 13 58 PM" src="https://user-images.githubusercontent.com/125219650/218337847-3af24924-d8d9-4efb-b4dc-995eb8a83371.png">

→ Average steps are 7500

→ Average calories burned are 2280

→ Average activity levels are highest in sedentary minutes. Users spend on average 16 hours in sedentary minutes, 3 hours lightly active, and only half hour in very/fairly active. 

Lastly, I wanted to observe what hours of the day users were most active by checking their total steps by hour. 

<img width="580" alt="Screen Shot 2023-02-11 at 5 23 45 PM" src="https://user-images.githubusercontent.com/125219650/218337913-8190aba5-e942-4f68-a417-4d6d16db73b5.png">

The top hours of steps recorded were early afternoon from 12-2pm and evening from 5-7pm. From this data, one can infer that users majority of the time either were active during their lunch hours or after work hours. 

## **PHASE 5: Share**

**The charts below summarize all of my key findings:**

<img width="590" alt="Screen Shot 2023-02-12 at 3 25 32 PM" src="https://user-images.githubusercontent.com/125219650/218343620-7d0b89ab-1f0c-49bc-8571-25f17d48bdd9.png">

**Key finding #1:** More users tended to log their activities for majority of the reporting period and were more active than those who less likely used their products.

<img width="670" alt="Screen Shot 2023-02-12 at 3 28 58 PM" src="https://user-images.githubusercontent.com/125219650/218343867-5650ffd4-996e-4965-9bdb-96bd471cc6b6.png">

<img width="712" alt="Screen Shot 2023-02-12 at 3 28 20 PM" src="https://user-images.githubusercontent.com/125219650/218343881-aaab7a2c-3d08-464e-b0b4-def86c46aec4.png">

**Key finding #2:** Sedentary users make up a significant portion of the data, spending on average 16 hours a day in sedentary minutes while only about 30 minutes in very active minutes. 

<img width="719" alt="Screen Shot 2023-02-12 at 3 36 19 PM" src="https://user-images.githubusercontent.com/125219650/218344061-46b40d0d-bc78-4838-9a0a-5f96459243eb.png">

**Key finding #3:** Users are most active during the 12-2pm and 5-8pm hours. Average usage time of the device is also approximately 21 hours. 

## **PHASE 6: Act**

**There is room for growth in this market and Bellabeat can strategize its marketing by following my recommendations below:**

→ Bellabeat can prolong the battery life of its Leaf wellness tracker since usage of products is majority of the day. 

→ Bellabeat can drive educational Health campaigns that encourage users to start having short active exercises daily throughout the day and eventually increase activity as consistency is obtained.

→ They should pair their campaigns with a stars-award incentive system that we see with most companies nowadays. Users who complete a 30 minutes workout each day for 7 days straight can receive Bellabeat stars and use those towards the Bellabeat membership or obtain their other products: Leaf, Time and Spring.

→ The Leaf product should start sending reminders to users who have been in a prolonged period of sedentary minutes. Similarly, it can also sync their heart rates to the app to keep track of heart activity and even signal healthcare services when an individual has taken a hard fall. 






















Citations:

Möbius. (2020, December 16). Fitbit Fitness Tracker Data. Kaggle. Retrieved February 1, 2023, from https://www.kaggle.com/datasets/arashnic/fitbit 
