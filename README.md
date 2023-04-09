# PowerBI_Portfolio
Here is the portfolio project on call centre trends for pwc Inc.

Here I had Showcased my skills by doing data analysing with the help of data visulisation tool (Microsoft PowerBI).


(The data set was given by a Switzerland Company PWC)

## Problem Statement:
Create a dashboard in Power BI for Manager that reflects all relevant Key Performance Indicators (KPIs) and metrics in the dataset.

Possible KPIs include (to get you started, but not limited to):

Overall customer satisfaction
Overall calls answered/abandoned
Calls by time
Average speed of answer
Agent’s performance quadrant -> average handle time (talk duration) vs calls answered

## Data Visualization
The Call Center Dashboard : Shows KPIs including overall customer satisfaction, overall calls answered/abadoned, calls by time, average speed of answer, agents performance quadrant -> average handle time(talk duration) vs calls answered

## Analysis
There are few quick measures used to get the certain insights:

- #Answered =  CALCULATE(COUNTA('Sheet1'[Call Id]), 'Sheet1'[Answered (Y/N)] IN { "Y" })
- #Resolved = CALCULATE(COUNTA('Sheet1'[Call Id]), 'Sheet1'[Resolved] IN { "Y" })
- #CR = DIVIDE([#Resolved], COUNTA('Sheet1'[Call Id]))
Two new columns are also created:
- Hour : To get the hourly number of calls
- AvgTalkDuration(sec): To get the time average talk duration in seconds



## Insights
- Average customer satisfaction rating: **3.40**
- Average Speed of Answering          : **67.52 Sec**
- Conversion rate- assign to resolve  : **73%**
- **Agents got least calls at 18th hour**
- **Dane is best performing agent**

![Call_Centre_Trends](https://user-images.githubusercontent.com/129333658/230790578-a67afaf7-550a-4d18-9736-54fd226aeffa.png)


