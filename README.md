# Hotel Data Analysis
## Table of contents
- [Project overview](#project-overview)
- [Data sources](#data-sources)
- [Tools](#tools)
- [Data cleaning/preparation](#data-cleaning/preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results/findings](#results/findings)
- [References](#references)


## Project overview

This data analysis project aims to solve business questions in order to analyze and visualize hotel booking data. Furthermore, build a visual data story or dashboard using Power BI to present to the stakeholders.

So, first we have two hotel types so it will be good to segment revenue by hotel type, also we want to understand if there is a trend for guest with personal cars and finally focus on average daily rate and guests to explore seasonality.

## Data Sources
Hotel Data: The primary dataset used for this analysis is the "hotel__revenue_historical.xlsx" file, containing detalied information about each guest since 2018 to 2020.

## Tools
- SQL server: Data cleaning and Data analysis
- Power BI: Creating report

## Data cleaning/preparation
1. Data loading and inspection
2. Handling missing values
3. Data cleaning and formatting

## Exploratory Data Analysis

The project has to answer the next 3 questions:
1. "Is our hotel revenue growing by year?" 
2. "Should we increase our parking lot size?"
3. "What trends can we see in the data?"

## Data Analysis
Include some interesting code/features worked with
``` sql
select arrival_date_year,
hotel,
sum((stays_in_week_nights + stays_in_weekend_nights)*adr) as revenue
from hotels
group by arrival_date_year, hotel
```
## Results/findings
The analysis results are summarized as follows:
1. The hotel revenue has been increasing per year for each type of hotel (City Hotel and Resort Hotel), a trend has been found during the years 2018 and 2019, however in 2020 there is a decreasing respect to 2019. It could be due to pandemic of COVID-19 during this year. The tourism was an affected industry.
2. There is not enough evidence to determine whether we should build a parking lot or not.
3. In the dashboard created using Power BI, we added filters which can help us to move throughout the years, verifying important information such a discount depending on the market segment, the average of adr, country, hotel type and specific period of time.

## References
1. Data Analyst Portfolio Project #1 | Build a Database | Develop SQL | Create a Dashboard [https://www.youtube.com/watch?v=S2zBHmkRbh]
2. SQL Tutorial [https://www.w3schools.com/sql/default.asp]
3. Big Data Analytics Lifecycle [https://www.informit.com/articles/article.aspx?p=2473128&seqNum=11&ranMID=24808]
