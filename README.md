# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

## Overview of Project

### Purpose

The main purpose was to use Excel to analyze different Kickstarter fundraising campaigns to compare them in relation to their launch dates and funding goals in order to give Louise information and insights to help her plan and set up her first crowdfunding campaign to help her fund her play "Fever." In order to do this, we needed to organize, sort, analyze crowdfunding data wanted create visualizations based on our findings. 

## Analysis and Challenges

First, I separated the "Category and Subcategory" column into two separate columns called "Parent" and "Subcategory" in order to help us get a more in-depth look at the data/ In addition, I created two other columns called "Date Created Conversion" and "Date Ended Conversion" in which we used the given Unix timestamps and converted them into Short Date form  to display the launch dates of the fundraisers. This also allowed me to look at the outcomes of campaigns by month and year easily. While the formula and conversion aspect of this part was not challenging, I still have trouble wrapping my mind around the concept of the Unix timestamps so I do not quite understand when an instance in which Unix timestamps would be more useful to use. 

### Analysis of Outcomes Based on Launch Date
![Theater Outcomes vs Launch](https://github.com/carolinacraus/kickstarter-analysis/blob/master/Theater_Outcomes_vs_Launch.png)

First,I created another column named "Years" in which I extracted the year from the "Date Created Conversion" column.Then, I created a pivot table with information about campaign outcomes filtered by the Parent Category "theater" and the new column I created, "Years." I filtered the column labels to only show the "successful," "failed," and "canceled" campaigns. Using this pivot table, I created a line chart which allowed me to visualize the relationship between outcomes and launch month. The most obvious observation I immediately noticed was that there had been no canceled theater outcomes in any of the months. The line chart also shows us that the month of May seems to have the most successful outcomes. 


### Analysis of Outcomes Based on Goals
![Outcomes vs Goals](https://github.com/carolinacraus/kickstarter-analysis/blob/master/Outcomes_vs_Goals.png)
![Outcomes vs Goals Chart](https://github.com/carolinacraus/kickstarter-analysis/blob/master/Outcomes%20Goals%20Chart.png)

For this analysis, I created a new sheet with a new chart to hold data for calculating and visualizing the percentage of successful, failed, and canceled plays based on their funding goal amount. The first column "Goals" holds dollar-amount ranges so projects can be ground based on their goal amount. The following columns are used for the calculations of number and percentage of successful. failed, and canceled campaigns. To populate these columns, I used the COUNTIFS() function. Using this data, I created a line chart to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y axis. 

### Challenges and Difficulties Encountered

The most challenging part of this analysis for me was the Outcomes Based on Goals pivot chart because changing the date ranges was meticulous and at first I made a few typo mistakes that were hard to follow. I also could not figure out if I can copy formulas the same way across columns as I can with rows so I think it took me longer to build the chart than it should have. I have also been having trouble consisitenly integrating the command line with my work and github but I plan on getting more familiar with those commands this week and practicing using it more. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

From my analysis of outcomes based on launch dates of campaigns, it seems that May is the month in which there are the most successful theater outcomes and there were no canceled theater outcomes in any of the months we looked at.In addition, it looks like December has the least successful outcomes as well as the most failed outcomes. 

- What can you conclude about the Outcomes based on Goals?

Based on my analysis about the Outcomes based on Goals, I noticed that the goal range of 1000-4999 had the most number of successful outcomes. However, I am unsure if I made a mistake somewhere that skewed my data because I feel like the percentage I calculated for the range 35000-39999 seems off but I could not figure out where I went wrong and did not realize it looked a little off until the last minute. It is also clear that as the goal range increases in amount, so do the number of successful outcomes as well as the number of total projects. 

- What are some limitations of this dataset?

There are many other factors that could affect the outcomes of the campaigns that were not considered. In addition, considering that the number of total campaigns each month differs, I am not sure if using percentages or this kind of visualization gives quite the right impression. 


- What are some other possible tables and/or graphs that we could create?
You could make a chart to compare the same month over different years as well in order to see if the outcome based on launch date is correlated with the percentage of success or failure. 
