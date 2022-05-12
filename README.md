# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends

## Overview of Project
The Kickstarter data set shows a set of campaigns in categories like film and video, theater, etc. and subcategories like television, plays, etc. which raise money in different counbtries. Each campaign and a goal and a pledged amount. The outcome ofthe campaign says if the goal amount is met or not.

Through the data set, we can determine whether or not the campaign succeeded (or canceld or live or failed), which category and subcategory the campaign belongs to and what impact factors like launch date, end date, country have on money raised in this campaign.

Louise’s play Fever came close to its fundraising goal in a short amount of time. In this project, she wants to know how different campaigns fared in relation to their launch dates and their funding goals which is what we analyse in deliverables 1 and 2. 

---

## Analysis and Challenges
### Deliverable 1
#### Analysis
- This deliverable thelps us visualize campaign outcomes in the parent category of "theater" based on launch date of the campaign.

![Theater_Outcomes_vs_Launch](https://github.com/preerit/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

- Across months, there is no trend for canceled theater campaigns. However the highest number of successful campaign appear to be around May. Failed campaigns seem to occur in months from May to August and in October

#### Challenges
- I did not encounter any challenges in Deliverable 1
- However I think the year, month, quarter split that happens when you pull the dates data into a pivot table could create some problems

### Deliverable 2
#### Analysis
- This deliverable is to help us visualize the percentage of successful, failed, and canceled plays based on the funding goal amount in the "plays" subcategory
- Sum() and Countifs() functions were the two Excel formulae that had to be used

![Outcomes_vs_Goals](https://github.com/preerit/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

- As the funding goal amount increases, the % of successful campaigns decreases and failed campaigns increases. There are no canceled campaigns in "plays" subcategory

#### Challenges
- The challenge that I faced was with flagging the goal amounts as 'less than 1000', '1000 to 4999', etc. Given the number of rows, I did not do it manually. I created a 'from goal amount' and 'to goal amount' columns in the 'Outcomes Based on Goals' sheet. Then I used countifs() formula using "<=" and ">=" combinations of lower and upper limit of goal amount data

---

## Results
### What are two conclusions you can draw about the Theater Outcomes by Launch Date?
* Across months, there is no increasing or decreasing trend for canceled theater campaigns - it is more or less stable, although there is no theater campaing canceled in October
* However the highest number of successful campaign appear to be around May. Theater campaigns in May have the highest chance of meeting their goal amount
* The number of successful and failed theater campaigns are the same in December. The probability is 50-50 for success and failure
* Failed campaigns seem to occur in months from May to August and in October. The least chances of failing are in months January, March, September and November

### What can you conclude about the Outcomes based on Goals?
* As the funding goal amount increases, the % of successful campaigns decreases and failed campaigns increases. There are no canceled campaigns in "plays" subcategory

### What are some limitations of this dataset?
* There are 19 records whose goal amount is greater than 1 Million currency
* The level of success across countries could be represented in colunmns
* The data could be sorted year wise

### What are some other possible tables and/or graphs that we could create?
* Outcome based on country 
* Count of campaigns across different categories in different countries
* Mean goal amount across different categories in different countries
* Median goal amount across different categories in different countries

