#   Google Data Analytics Capstone: Cyclistic Case Study
Course: [Google Data Analytics Capstone: Complete a Case Study] 
## Introduction
In this Case Study, I will demonstrate my skills obtained through my time with the Google Data Analytics course in the real-world task of a junior data analyst at a fictional company, Cyclistic. In order to answer the critical business question, I will follow the steps of data analysis of Ask, Prepare, Process, Analyze, Share, and Act. 

## Background
### Cyclistic
A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day.   
  
Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members.  
  
Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno (the director of marketing and my manager) believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs.  

Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends.  

### Scenario
I am assuming to be a junior data analyst working in the marketing analyst team at Cyclistic, a bike-share company in Chicago. The director of marketing believes the company’s future success depends on maximizing the number of annual memberships. Therefore, my team wants to understand how casual riders and annual members use Cyclistic bikes differently. From these insights, my team will design a new marketing strategy to convert casual riders into annual members. But first, Cyclistic executives must approve our recommendations, so they must be backed up with compelling data insights and professional data visualizations.

## Ask
### Business Task
Devise marketing strategies to convert casual riders to members.
### Analysis Questions
Three questions will guide the future marketing program:  
1. How do annual members and casual riders use Cyclistic bikes differently?  
2. Why would casual riders buy Cyclistic annual memberships?  
3. How can Cyclistic use digital media to influence casual riders to become members?  

Moreno has assigned me the first question to answer: How do annual members and casual riders use Cyclistic bikes differently?
## Prepare
### Data Source
I will be using Cyclistic's historical trip data to analyze and identify trends from Jan 2022 to Dec 2022 which can be downloaded from [divvy_tripdata](https://divvy-tripdata.s3.amazonaws.com/index.html). 
This is a public data set that can be used to explore how different customer types are using Cyclistic bikes. Though it should be noted that data-privacy issues prohibit from using riders' personally identifiable information. This means we cannot determine whether or not casual have bought multiple single passes. 
### Data Organization 
There are 12 files with the naming convention of YYYYMM-divvy-trip data and each file includes information for one month, such as the ride_id, bike type, start time, end time, start station, end station, start location, end location, and whether the rider is a member or not. The columns names are ride_id, rideable_type, stared_at, ended_at, start_station_name, star_station_id, end_station_name, end_station_id, start_lat, start_lng, end_lat, end_lng and member_casual. 

## Process
I started my process in Google Sheets. Some of the files were simply too big to be uploaded so I split the CSV files and then combine them again after I was done with the cleaning. This made the process more manageable in the long run. My first step was to gather more relevant data using the formula of =WEEKDAY (C2, 1) to calculate a new column named day_of_week. Then used another formula of =D2-C2 to determine the ride_length. Formating to duration to calculate how long each of the rides was.
### Data Cleaning
1. All rows having missing values are deleted.
2. Trips with a duration of less than a minute and longer than a day are excluded.
3. End row count is 101,825


## Analyze and Share
Data Visualization: [Tableau](https://public.tableau.com/views/CapstoneProject-Cyclist/Story1?:language=en-US&:display_count=n&:origin=viz_share_link)
The stat is stored appropriately and is now prepared for analysis. I have made multiple pivot tables and visualized them in Tableau. 
The analysis question is: How do annual members and casual riders use Cyclistic bikes differently?

First of all, I compared the casual riders vs members each month and what days they use them most. 
![image](https://i.imgur.com/j92ds19.png)
![image](https://i.imgur.com/NUSsLTP.png)
![image](https://i.imgur.com/2nc4KzK.png)

__Months:__ When it comes to monthly trips, both casual and members are very similar in behavior, with far more trips in the spring and summer, when the weather is nicer and fewer in the winter. While there is a significant gap between casual and members most of the time. The gap does get the closest to closing during the months of July and August. Perhaps due to the influx of people not from the city. 
__Days of Week:__ When the days of the week are compared, keep in mind for these graphs 1 is Sunday and 7 is Saturday. 

We can infer from these graphs that members may be using bikes for commuting to and from work on the weekdays while casual riders are using bikes throughout the day, more frequently over the weekend, and during summer months.

This hypnosis can also be further solidfied when looking at the average trip length between members and casual riders. 

![image](https://i.imgur.com/KexwLFZ.png)

Summary:

Casual: Prefer to use the bikes for longer periods of time, more often in the spring and summer and on weekends. They also tend to have longer trips, then members. 
Members: Tend to take short trips during the week during the time of commuting too and from work, still during the spring and summer with a small amount in the winter months. 

## Act
After identifying a couple of differences between the two different riders I have concluded some ideas as to how to create more members from the casual riders. 
1. The best time to recruit new members would be during the spring/summer when the volume of riders is the highest.
2. Casual riders are more active during the week so might be more intrigued by the idea of a weekend pass and since it is most popular during the spring and summer a seasonal pass.
3. Current members tend to use bikes for short periods while casual use them for longer periods. Offering discounts to members for longer trips to make the membership, more worth it in their eyes. 






