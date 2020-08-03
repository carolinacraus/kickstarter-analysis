# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends

## Overview of Project

### Purpose

The main purpose was to use Excel to analyze different Kickstarter fundraising campaigns to compare them in relation to their launch dates and funding goals in order to give Louise information and insights to help her plan and set up her first crowdfunding campaign to help her fund her play "Fever." In order to do this, we needed to organize, sort, analyze crowdfunding data wanted create visualizations based on our findings. 

## Analysis and Challenges

First, I separated the "Category and Subcategory" column into two separate columns called "Parent" and "Subcategory" in order to help us get a more in-depth look at the data/ In addition, I created two other columns called "Date Created Conversion" and "Date Ended Conversion" in which we used the given Unix timestamps and converted them into Short Date form using the YEAR() function to display the launch dates of the fundraisers. This also allowed me to look at the outcomes of campaigns by month and year easily. While the formula and conversion aspect of this part was not challenging, I still have trouble wrapping my mind around the concept of the Unix timestamps so I do not quite understand when an instance in which Unix timestamps would be more useful to use. 

### Analysis of Outcomes Based on Launch Date
![Theater Outcomes vs Launch](https://github.com/carolinacraus/kickstarter-analysis/blob/master/Theater_Outcomes_vs_Launch.png)

First, I created a pivot table with information about campaign outcomes filtered by the Parent Category "theater." Using this pivot table, I created a line chart which allowed me to visualize the relationship between outcomes and launch month. 


### Analysis of Outcomes Based on Goals
![Outcomes vs Goals](https://github.com/carolinacraus/kickstarter-analysis/blob/master/Outcomes_vs_Goals.png)

For this analysis, I created a new sheet with a new chart to hold data for calculating and visualizing the percentage of successful, failed, and canceled plays based on their funding goal amount. The first column "Goals" holds dollar-amount ranges so projects can be ground based on their goal amount. The following columns are used for the calculations of number and percentage of successful. failed, and canceled campaigns. To populate these columns, I used the COUNTIFS() function. Using this data, I created a line chart to visualize the relationship between the goal-amount ranges on the x-axis and the percentage of successful, failed, or canceled projects on the y axis. 

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
