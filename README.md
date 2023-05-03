# Crowdfunding Campaigns Project
## Overview


The objective of this project is to address a number of inquiries concerning the creation of crowdfunding campaigns, with a particular focus on identifying the specific factors that influenced the development of campaigns with an approximate budget of $10,000. To achieve this objective, an extensive analysis of several thousand crowdfunding campaigns was conducted.

### The Dataset 

- Crowdfunding Campaigns source [Dataset](
https://raw.githubusercontent.com/lindaperez/kickstarter_analysis/main/data.csv)

Significant Column Meanings:

The Goal: This column represents the required funds for each campaign to achieve its objectives.
The Pledged: This column indicates the actual amount of money raised by each campaign.
The Outcomes: This column highlights whether a campaign has achieved its goals or not.
The Country: This column records the country where the campaign originated.

Limitations:

There was no data dictionary available for this dataset, and some columns were interpreted intuitively.
Certain columns, such as spotlight or staff_pick, have limited information that could provide more insights when analyzed in conjunction with the outcomes.


## Analysis

Prior to finding a solution, it was essential to consider the potential questions that could be addressed based on the characteristics and significance of the data:

What is the optimal timing for launching a specific crowdfunding campaign?
Is creating a crowdfunding campaign with a budget of $10,000 a strategic decision? Are there any correlations between the campaign goal and its success rate? Would setting a higher or lower budget be more effective?


### Analysis of Outcomes Based on Launch Date

To resolve this case,  how to address the specific questions posed were considered. This included determining the optimal time to launch a crowdfunding campaign and identifying the relationship between launch dates and outcomes. To achieve this, we analyzed data over time and examined the success, failure, and cancellation rates of campaigns, particularly over the years.

To compare how the months were distributed over the years, we present the following table and chart:

<img width="1205" alt="Screen Shot 2022-07-21 at 1 17 43 PM" src="https://user-images.githubusercontent.com/1729991/180308205-2d2e4cfc-5571-4c0e-b51f-e0315fdcad93.png">

The pivot table shows a peak in May, representing the month in which campaigns have been most successful over the years.
The pivot chart, titled "Theater Outcomes Based on Launch Date," displays a line chart with several points, one of which highlights May as the most successful month to launch a campaign, with 111 out of 166 campaigns achieving their goals. In contrast, the chart indicates that December is the least favorable month to launch a campaign, with only 35 successful campaigns out of 75 launched during this month.


### Analysis of Outcomes Based on Goals



Here's a more formal and corrected version of the text:

Several questions were addressed during the analysis, including whether a budget of $10,000 is a strategic choice for creating a crowdfunding campaign, whether a lower or higher budget would be more effective, and if any relationship exists between budget and successful campaigns.

Outcomes, such as successful, failed, and canceled, were displayed in conjunction with goal ranges or budget ranges to gain an understanding of how many projects were successful within each budget range. For instance, within a budget range of $10,000 to $14,999, there were 39 successful projects out of 72. To present the data in a more readable format, percentages were utilized.

Upon examination, it was found that within the budget range of $10,000 to $14,999, approximately 54% of projects were successful, while 46% were not. The question remains as to whether this budget range is optimal for the project.

To address this question, a table was created, indicating the range of possible goals or budgets, the number of successful, failed, and canceled projects, and their corresponding percentages.


![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


## Conclusions


The view "Analysis of Outcomes Based on Launch Date" provides the way to answer our first fundamental question: What is the best time to create a "Play" Crowdfunding Campaign based on the Parent category "Theater" over the years from 2009 and 2017. 

	- The best time is in May. May is the best month to launch a Campaign. After this, the second one would be between April, May and some days of June. After May the amount of outcomes start falling until January of the next year where they start increasing again. 

	
The view Analysis of Outcomes Based on Goals provides the way to answer our second fundamental question: Will the campaign be able to reach the goal expected, at least $ 10.000? 

	- No, Having a budget of $10000 is hard to get with only 54% of the cases approved.

The projects with a budget less than $1000 are the most successful with a 76% of assertiveness over the years. After it, it could be a better idea to reduce the budget to a range between $1000 to $4999 due to 73% of those projects got the whole budget. If the customer can not reduce the budget to that amount, something that can help is to have a greater budget, between 35000 and 44999, those projects were successful in 67% of the cases.

## Additional Analysis

To unhide more patterns to create more successful campaigns there are some additonal questions that were explored:

	1. Creating the campaign in a different country may help funding the goal budget?

		It can be created a table with outcomes and countries and determine what is the country with the most successful projects by "Play" subcategory.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Outcomes_by_Country.png)


	2. How long should the campaign be? 
		It cab be created a column with the number of days that every campaign last and create a table with the average of days that every campaign had, filtered by subcategory "Plays"  
		Then, It can be seen that the average days for the most successful campaigns is 28.5days, with 412 successful projects.
		
![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Size_by_Outcomes_Country.png)
