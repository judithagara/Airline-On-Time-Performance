# Airline On-Time Performance Data Exploration 

## Dataset

> **Dataset Description:** This dataset reports flights in the United States, including carriers, arrival and departure delays, and reasons for delays in the year 2006. It also contains data on airports and airplanes. Four (4) tables/.csv files are used in this analysis. They include:

> 1. **2006.csv** - flights report in the year 2006 **(7141922 rows, 18 cols)**.
2. **carriers.csv** - airline information **(1491 rows, 2 cols)**.
3. **airports.csv** - airport information such as city, state, country, latitude and longitude **(3376 rows, 7 cols)**.
4. **plane-data.csv** - plane info such as type, manufacturer, model, engine type, etc. **(5029 rows, 9 cols)**.
 
> All files are available for download [here](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/HG7NV7)


After preliminary wrangling, I had a master dataset of **5,503,507** records (rows) and **18** features (columns) distributed across quantitative and qualitative datatypes.


## Summary of Findings

- In the exploration, I found that scheduled flights are generally successful: **72.73%** on time, **26.67%** delayed and **0.61%** cancelled. I also found that the most common reason for flight cancellation is the **carrier** (airline) and least common reason is **security**, accounting for only 0.14% of the cancel cases.

- Looking at the distribution of delay time in minutes showed a multimodal distribution having three(3) peaks after a log transform was applied to the y-axis. The distribution of arrival and departure delays are closely resemble.

- The distribution of distance is a right-skewed one. Most flight distances are between **11 - 711 miles**, with the most occuring between **211 - 311 miles**. The distribution suggests some outliers between about **3000 - 5000 miles**.

- Most flights are scheduled between Early Morning - Evening **(4am - 8pm)**. Very few are scheduled at Night **(between 8pm - midnight)** and flights are seldom scheduled **after midnight**.

- **36%** of Evening flights and **31%** of Noon and Night flights are delayed. **23%** of morning flights are delayed, **21%** of late night flights are delayed and **15%** of morning flights are delayed.

- **Evening, night and noon flights** are the most cancelled.

- **Atlantic Southeast Airlines** has the most delays (over 36%). It is followed be **American Eagle Airlines** with about 30% of scheduled flights delayed. **Mesa Airlines** followed by **Atlantic Southeast Airlines** has the most cancellations.

- When considering percentages of delay per city, **Newark** tops the list while **Atlanta, New York, Chicago** are tied for origin airports. They are followed by Detroit. In the case of destination airports, the list goes from **Newark - New York - Chicago - San Francisco - Atlanta**.

- When considering the percentages of cancellation per city, we see that **Atlanta** tops the list followed by **New York, Detriot and Chantilly** for origin airports. In the case of destination airports, the list goes from **Atlanta - Chantilly - Detroit - New York - Phoenix** which closely follows New York.

- Departure delays across all week days are between **33 - 40 minutes** long. Arrival delays follow a downward trend from Monday to Thursday (about 4 mins) and peaks on Saturdays (to about 23 mins) and drops to 5 mins on Saturday. 

- Departure delays across all months are between **30 - 40 minutes long**. Arrival delays on the other hand follows a downward trend with significant drop in June and July and a spike in September.


## Key Insights for Presentation

For the presentation, I focus on presenting plots that answer the following questions:
- When is the best time of day/day/week/time of year to fly to minimise delays? 
- What is the top reason for flight cancellations?
- Are there certain airlines that are home to more delays or cancellations?

After some computations, I use simple bar charts to summarize and illustrate the answers. Bar charts provide the clearest representation of these insights.
