# Bellabeat-Casestudy
Bellabeat is a high-tech manufacturer of health-focused products for women.

Bellabeat is successful small company,but they have potential to become larger player in the global smart device market. As a junior data analyst i will be working on the marketing analyst team to analyze smart device fitness data that could help unlock new growth opportunities for the company. I have been asked to focus on one of Bellabeat products and analyze smart device data to gain insight into how consumers are using their smart devices.These insights will help to guide marketing stategy for the company. You will present your analysis to the Bellabeat executive team along with your highlevel recommendations for Bellabeat's marketing strategy. In order to answer key business questions I have followed 6 steps of analysis process - Ask,Process,Prepare,Analyze,Visualize,Act.

1.Ask
1.1 Business Task: Analyze smart device data to gain insight into how consumers are using their smart devices.These insights will help to guide marketing strategy for the company

1.2 Key stakeholders:

Urška Sršen: Bellabeat’s cofounder and Chief Creative Officer Sando Mur: Mathematician and Bellabeat’s cofounder; key member of the Bellabeat executive team.

2.Process
2.1 Dataset:
● FitBit Fitness Tracker Data (CC0: Public Domain, dataset made available through Mobius):
 * This Kaggle data set contains personal fitness tracker from thirty fitbit users.
 * Thirty eligible Fitbit users consented to the submission of
   personal tracker data, including minute-level output for physical activity, heart rate, and sleep monitoring. 
 * It includes information about daily activity, steps, and heart rate that can be used to explore users’ habits.
2.2 Files:
    There are 18 files stored in .csv file formats.For analysis purpose only 6 files are used.
     1.dailyActivity_merged.csv
       This file contains details about Activity date,active minutes,total distance,total steps and Calories burned.
     2.dailyCalories_merged.csv
      This file contains data about calorie burnt for particlular day.
     3.dailyIntensities_merged.csv
       This file contains details about active minutes spent whole day and distance covered.
     4.dailySteps_merged.csv
       This file contains details about total steps count for particular day.
     5.sleepDay_merged.csv
        This file contains information about total sleep records,total time in bed.
     6.weightLogInfo_merged.
       This file contains users weight,fat and BMI.
2.3 Limitations:
    Since there are only 30 users data,it is difficult to carry out thorough analysis.

3.Prepare
I used Google Sheets and Bigquery for data cleaning.All the 6 csv files were opened in Google Sheets and checked for anamolies,Except sleepDay_merged and weightLogInfo rest other files are clean and accurate.
The following steps were taken to clean the two files:
1)checked for any duplicate entries in both files,there were 3 duplicate entries found in sleepDay_merged file and removed from the file.
2)Date and sleepDay fields in weightLogInfo_merged and sleepDay_merged files were incorrectly formatted.so those fileds were formated to custom date and time ,now only Date is shown irrespective of time(Am/PM).
3)All the files were loaded to Bigquery to check for unique entries in each file for users.
    There were 
    33 entries for users in dailyActvity_merged 
    33 entries for users in dailyCalories_merged
    33 entries for users in dailyIntensities
    33 entries for users in dailySteps_merged
    24 entries for users in weightLogInfo_merged 
    8 entries for users in sleepDay_merged.
    Since weightLogInfo_merged has 24 and sleepDay_merged has only 8 records it is difficult to carry out analysis with insufficient data which may result in wrong analysis.
4.Analyze
 Now that the data is cleaned and uploaded to bigquery,next step is analyzing the data.The analysis includes querying daily                              activities,calories,totalsteps,weightLog and sleep patterns.
 
5.Share
I used Tableau for data visualization.

6.Act
From the above analysis and data visualization it is clear that active minutes spent and calories burnt result in active life style. which inturn helps in maintaining BMI and have quality sleep.

Conclusion and Recommendation:
Conclusion:
only 24 out of 33 tracked their weightlog data and 8 out of 33 tracked their sleep data.so it is clear from the analysis that we need to focus more on analyzing activity data rather than sleep and weightlog data.

Recommendation:
1.Include Demographic data since bellabeat is focused mainly on women's health.

2.Ideal steps for maintaining good life style is 10000,so notify users how many steps recommended and keep reminding them to walk on regular basis.At the end of the day encourage users by giving badges on their achievement.

3.Drinking water is essential for good health,so keep notifying users on regular intervals to drink water.

Tableau public link -  https://public.tableau.com/app/profile/asha7854/viz/Bellabeatcasestudy_166738084 13030/Story1?publish=yes  
