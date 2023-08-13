# Citi Bike Analysis with Tableau

## Background 
Congratulations on your new job! As the new lead analyst for the [New York Citi Bike](https://en.wikipedia.org/wiki/Citi_Bike) program, you are now responsible for overseeing the largest bike-sharing program in the United States. In your new role, you will be expected to generate regular reports for city officials looking to publicize and improve the city program.

Since 2013, the Citi Bike program has implemented a robust infrastructure for collecting data on the program's utilization. Each month, bike data is collected, organized, and made public on the [Citi Bike Data](https://citibikenyc.com/system-data) webpage.

However, while the data has been regularly updated, the team has yet to implement a dashboard or sophisticated reporting process. City officials have questions about the program, so your first task on the job is to build a set of data reports to provide the answers.

## Deployment
Please find below the link to the Tableau dashboard, showcasing the results of the analysis: 
https://public.tableau.com/app/profile/simon.gomes/viz/citibike_16918929176210/Home
    
## Data Source
1. The initial stage of the project involved acquiring all the monthly CSV files, covering the period from January 2018 to December 2020, from the [Citi Bike Data](https://citibikenyc.com/system-data) webpage and organizing them in a designated folder named "data". The data used in this analysis specifically pertains to the Jersey City region.
2. Subsequently, I established a Jupyter Notebook file, named "[citibike.ipynb], to systematically clean and combine all the monthly CSV files into a single CSV file, in preparation for importing into Tableau.
3. The following is a comprehensive overview of the data cleansing process:
   
   * First import pandas.  
   * Read in all csv files for a single year in a pandas dataframe, store in a list, and then concatenate into a single dataframe.
   * Repeat step for the remaining years.   
   * Combine all three dataframes into a single dataframe.
   * Change the values in the gender column from the numerical value to the actual value. 
   * Then save the dataframe to a csv file.
   
   **Please note that the large size of the CSV files precludes their storage in this repository and in GitHub's Large File Storage. As a result, the CSV files have been added to a .gitignore file.**
   
## Dashboards
From the Citi Bike data, a homepage and three corresponding dashboards were created to provide a comprehensive analysis and visualization of the data.

### Homepage
* The homepage serves as an introduction to the project, providing a concise overview of its purpose and contents. It clearly summarizes the key insights and findings of each dashboard, allowing for quick and easy navigation.


### User Analysis 
* The dashboard presents a comprehensive analysis of the Citi Bike trips, taking into account various factors such as user type, gender, and age. Additionally, it provides an in-depth examination of trip patterns based on the hour of day and day of the week, as well as the total number of trips per month.


### Station Analysis
* The dashboard focuses on the analysis of trips in relation to the bike stations. It compares the trip patterns between weekdays and weekends and provides insights into the average trip duration for each month.


### Geographic Analysis
* The third dashboard features two maps showcasing the geographical locations of the start and end stations. The size and color of the markers are used to represent the total number of trips that originated or terminated at each station, providing a visual representation of the trip patterns and frequency.


## Summary


* An evaluation of the data covering the time period from 2018 to 2020 shows a total of 1,095,641 trips made using bicycles in New York City. This represents a decrease of 4.83% over the three-year period. The observed decline in trips can be attributed to the adverse effects of the COVID-19 pandemic, including the associated shutdowns, on the usage of bicycles.
* A comparison of the data from 2018 to 2020 reveals a decrease of 30.20% in the number of subscribers, while there was a simultaneous increase of 374.90% in the number of customers. This disparity in trends can be attributed to the impact of the COVID-19 pandemic on the usage of bicycles in New York City.
* Over the specified time period, there appears to be a positive trend in the number of female riders, with an increase of 12.55%, while the number of male riders has decreased by 22.29%. While the reason for this trend is not definitively known, it could potentially be attributed to improved safety and security measures for female riders. Further analysis would be required to establish this hypothesis.
* It is noteworthy that the peak utilization of citibikes in New York City occurs during the weekday, specifically during the hours of 8 a.m. and 5 p.m., as a significant number of commuters utilize bicycles for their daily commute.
* An examination of the data reveals that the pattern of peak bicycle usage in New York City remained consistent during 2018 and 2019, with the busiest periods occurring during the weekdays. However, in 2020, a notable deviation from this trend emerged, with weekends experiencing the highest levels of bicycle usage. This shift can likely be attributed to the widespread adoption of remote work as a result of the COVID-19 pandemic.
  
* A review of the data by month reveals that the highest usage of bicycles in New York City occurs during the summer months of July, August, and September, in comparison to the winter months. In April of 2020, a marked decrease in bicycle usage was observed, which can be attributed to the restrictions imposed during the early stages of the COVID-19 pandemic.

* The analysis of the data indicates that the majority of bicycle riders in New York City belong to the age group of 29 to 43, with a prevalence of male riders among this demographic.

* An examination of the data reveals a disparity in the number of start stations compared to the number of end stations.

* The analysis of the data, as depicted in the chart, indicates that Grove St PATH and Hamilton Park are the most frequently used stations for both starting and ending trips.

* An examination of the graph presenting the average trip duration, measured in minutes, per month reveals a noteworthy increase in 2020 compared to the average trip durations in 2018 and 2019. This deviation can be attributed to the closure of businesses and an increased amount of time spent outdoors, particularly during the summer months, as a result of the COVID-19 pandemic. 

* An analysis of the start station map highlights the concentration of the most frequently used stations in Jersey City, New Jersey, primarily in the zip codes 07302 and 07310. This suggests that the residents of Jersey City utilize the bicycle-sharing service extensively, potentially due to its cost-effectiveness when compared to other transportation options, such as taxis and ride-sharing services.

* Similar to the start station map, the end station map also illustrates a notable concentration of the most frequently used stations in Jersey City, New Jersey, indicating that residents are likely utilizing the bicycle-sharing service for their commutes to and from work. 

## Conclusion
In conclusion, this Tableau analysis provides a comprehensive overview of the trends and patterns in Citibike usage over a specified time period. Through the creation of interactive dashboards and visualizations, key insights have been extracted and presented, highlighting trends in user type, gender, and age, as well as trip patterns based on hours and weekdays. One noteworthy phenomenon observed from the overall analysis is the high usage of the Citibike service by residents of Jersey City, New Jersey, primarily for commuting purposes. This analysis serves as a valuable resource for anyone interested in understanding the usage of Citibike and exploring the data behind this popular bike-sharing service. I hope that this work will inspire further research and investigation into the data, and encourage others to build upon the insights presented here.
