# An Analysis of Kickstarter Campaigns

# Overview of Project
* We will be performing data analysis on several hundred crowdfunding projects to uncover any hidden trends. The projects for Challenge #1 include theater plays. The campaign outcomes are visualized based on their launch dates and their funding goals. 
### Purpose
Louise’s has a theater play project for which she is seeking funding from sponsors. We are trying to help her to investigate if chance of success for her play funding can be increased by selecting an optimized launch date or by adjusting the size of the budget for the play.  In other words, she wants to know how different campaigns fared in relation to their launch dates and their funding goals.  We will also learn some useful tools in Excel including pivot tables, filtering, and plotting to help with our analysis. 
## Analysis and Challenges
We selected a subset of total projects in “theater” category, and “plays” subcategory using pivot tables. In addition, we classified our data further based on "launch date" and amount of funding "goal" using pivot tables and "countifs" function in Excel. We first tabulated and plotted total number of successful and failed projects versus the month in which the projects launched. (Month is obtained from "converted date").  We examined the trend for number of successful projects versus the launch date (month) to check if there is any correlation between chance of success or failure and the month in which it is launched.  In second step, we plotted the number of successful and failed projects versus the amount of funding "goal" to identify patterns.  

### Analysis of Outcomes Based on Launch Date

Count of outcomes	Column Labels			
Row Labels	successful	failed	canceled	Grand Total
Jan	56	33	7	96
Feb	71	39	3	113
Mar	56	33	3	92
Apr	71	40	2	113
May	111	52	3	166
Jun	100	49	4	153
Jul	87	50	1	138
Aug	72	47	4	123
Sep	59	34	4	97
Oct	65	50		115
Nov	54	31	3	88
Dec	37	35	3	75
Grand Total	839	493	37	1369
 

### Analysis of Outcomes Based on Goals
Goal	Number Successful	Number Failed	Number Canceled
less than 1000	141	45	0
1000 to 4999	388	146	0
5000 to 9999	93	76	0
10000 to 14999	39	33	0
15000 to 19999	12	12	0
20000 to 24999	9	11	0
25000 to 29999	1	4	0
30000 to 34999	3	8	0
35000 to 39999	4	2	0
40000 to 44999	2	1	0
45000 to 49999	0	1	0
50000 or more	2	14	0

 

### Challenges and Difficulties Encountered
* To produce the second deliverable (Outcomes based on Goal) the instructions were confusing as it seems it wants to use “filter” and “count if” to produce the table. It is not clear if you use “filter” how you can create the requested tables.  The text is very vague here:

> Use COUNTIFS() functions to populate the "Number Successful," "Number Failed," and "Number Canceled" columns by filtering on the Kickstarter "outcome" column, on the "goal" amount column using the ranges created in Step 3, and on the "Subcategory" column using "plays" as the criteria.

I eventually had to write  a separate formula for 36 cells in requested table using countifs function. But I don’t think that’s an elegant approach. 
## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?

* The data indicates while numbers of failed projects remain relatively constant, number of successful projects (and as result percentage of successful project as fraction of total projects) gradually increases to peak in May and then declines by the end of the year. This data suggest campaigns launching between April and July have a higher chance of success. 
* Number of successful projects remains always higher than the number of failed projects indicating a success chance of greater than 50% throughout the year. The success chance reduces as we approach the end of the year and minimizes to 50% at December.
* The data indicates number of cancelled projects remains a small fraction of total projects and remains constant throughout the year suggesting the launch date does not have much impact on cancellation. 


### What can you conclude about the Outcomes based on Goals?
* The data indicates there is not a clear linear relationship between the “Goal” amount and chance of success of the projects. Clearly very small projects (with funding goals < 5000) have the highest chance of success, but also projects with funding between 35000 and 45000 also have a relatively high chance of success (67%). 
 High chance of success for small projects might be explained by the fact that it is easier to find sponsors for small projects probably because there are more sponsors with small funds out there. High rate for success for projects between 35000 and 45000 is based on only a limited number of projects (total 9 projects fall in these classes). So, one need to be cautious to generalize these results.
* Clearly projects with funding greater than 50000 have a very high chance of failure. This can be explained by the fact that there are fewer sponsors who have that much money out there. 


### What are some limitations of this dataset?
* The dataset is biased toward smaller projects (small fund goal). It is hard to generalize trends for mid size and larger projects.

### What are some other possible tables and/or graphs that we could create?
* It will be useful to create plots of “percentage” of successful and failed projects with respect to total projects. 
* It will be useful to plot number of backers to examine if it is correlated with success rate
* It will be useful to plot the ratio of “pledged” to “goal” to examine the rate of success as a continuous function versus a binary (success or fail)


