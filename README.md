# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends

## Overview of Project

The Kickstarter data set shows a set of campaigns in categories like film and video, theater, etc. and subcategories like television, plays, etc. which raise money in different counbtries. Each campaign and a goal and a pledged amount. The outcome ofthe campaign says if the goal amount is met or not.

Through the data set, we can determine whether or not the campaign succeeded (or canceld or live or failed), which category and subcategory the campaign belongs to and what impact factors like launch date, end date, country have on money raised in this campaign.

Louise’s play Fever came close to its fundraising goal in a short amount of time. In this project, she wants to know how different campaigns fared in relation to their launch dates and their funding goals which is what we analyse in deliverables 1 and 2. 

---

## Analysis and Challenges
### Deliverable 1
### Deliverable 1 Analysis

- This deliverable thelps us visualize campaign outcomes in the parent category of "theater" based on launch date of the campaign.

- Across months, there is no trend for canceled theater campaigns. However the highest number of successful campaign appear to be around May. Failed campaigns seem to occur in months from May to August and in October

![Theater_Outcomes_vs_Launch](https://github.com/preerit/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Deliverable 1 Challenges

- I did not encounter any challenges in Deliverable 1

- However I think the year, month, quarter split that happens when you pull the dtes data into a pivot table could create some problems

### Deliverable 2
### Deliverabel 2 Analysis

- This deliverable is to help us visualize the percentage of successful, failed, and canceled plays based on the funding goal amount in the "plays" subcategory

- Sum() and Countifs() functions were the two Excel formulae that had to be used

![Outcomes_vs_Goals](https://github.com/preerit/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)
