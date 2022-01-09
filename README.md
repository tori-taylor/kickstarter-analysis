# Kickstarting with Excel

## Overview of Project

### Purpose
The purpose of the assignment was to analyze the success rates of theater kickstarter campaigns, specifically plays. The insight gained from this analysis would ideally help Lousie understand why her play Fever did not reach it's fundraising goal. In addtion the analysis would potentially find common attributes (goals, timing etc) within successful play campaigns so Louise can adopt these atrributes when planning for her next play.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
The Analysis first looked at success rate of theater productions (considered a success if the campaign hit it's fundrasing goal)  by month. The purpose of this was to determine if certain months of the year were better to launch a theater campaign. This chart shows theater outcomes by launch month. ![Theater_Outcomes_vs_Launch](https://github.com/tori-taylor/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)
A high level explanation of how this chart was completed was by: 
- breaking out the CATEGORY & SUBCATEGORY in the data set to PARENT CATEGORY and SUBCATEGORY so that theatres as a parent category could easily be extracted from the data set
- the launch date was converted into a readable format so the chart could be plotted by month
- creating a pivot table for the desired data
- creating a line chart
### Analysis of Outcomes Based on Goals
This looked at outcomes of plays based on the fundrasing goal of the project. The purpose of this was to see if goal was a determinent of campiagn success. 
![Outcomes_vs_Goals](https://github.com/tori-taylor/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
This was created by making buckets based on goals (for example $1000 to $4999)
- Using a countif function to count how many plays were successful / failed / cancelled for that specific goal range
- Finding the percent success / failed / cancelled for each bucket
- Plotting the data collected above with a line chart
### Challenges and Difficulties Encountered
I had no challenges with creating the line chart for analysis based on launch date. However possible issues could be using the incorrect range of data in the source for the pivot table therefore not captuing the full data set, incorrectly converting the dates and therefore making "month"not an avialble x acis, or instead doing a "count of outcomes"as your value in the pivot table doing an "sum" or "average".
I had no issues creating the analysis for outcomes based on goals. An issue could have been if the countif function for bucket 1000 to 4999 was counting "greater than or equal to 1000" and "less than or equal to 4999", and bucket 5000 to 9999 was counting greater than or equal to 5000" and "less than or equal to 9999" you would have an issue if a goal was 4,999.50 as it would not get counted in either bucket.
## Results
Looking at the graph for theatre outcomes based on launch data we can conclude that May has the highest success rate and December has the lowest success rate. From the analsis for outcomes based on goal it appears that lower goals have a higher sucess rate compared to higher goals. There are several liminiations for the data set. One, there are very few high goal plays (only four over 40,000) therefore it is likely not a big enough pool to confidently say that high goal plays will not succeed. Most importantly we are unaware of how these campiagns were run, who marketed them how they were marketed etc. We also are unaware if public interest in differet types of plays could be causinng a sucess or failutre. The data set does not include things like, play location, casting etc all that may lead to if doners are more interested in making a pledge. For the line chart showing outcomes based on goal, I would have chosen a stacked bar chart, as the two lines represent a % of the same number. Therefore a single bar with each percent would better visualize that they are repsenting the % of one number. Since we have end data we should also be looking at success rate based on how long the campaign was run as an anlysis. Another analysis is to look at success rates by country.
