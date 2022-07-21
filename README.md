# Crowdfunding Campaigns Project Analysis

## Overview of Project
### Purpose

Having several thounsand of Crowdfunding Campaigns, Were answered a decisive variety of questions for the creation of a crowdfunding campaign, most specifically were determined the specific factors that influenced the creation of a campaign with an estimated budget of $10.000. 



### The Dataset 

- Crowdfunding Campaigns source [Dataset](
https://raw.githubusercontent.com/lindaperez/kickstarter_analysis/main/data.csv)

Most important columns meaning:

    - The Goal: how much money each campaign will need to succeed.
    - The Pledged: how much each campaign actually made.
    - The Outcomes: does the campaign met its goal.
    - The Country: lists the country in which the campaign was started.

- Limitations:

	- No data dictionary found, some columns were used in a intuitive way
	- There is not much information about some columns like spotlight or staff_pick, that can give more information to correlate it with the outcomes. 
	- There is not much information about the quality of the data, we guess it is consistent. 


## Analysis

Before encounter a solution, it was important to think about the questions that might be answered based on the characteristics and meaning of the data:

1. When is the best time to launch the specific Campaign? 

2. Is it a strategic decision to create a crowdfunding with that particular budget $10.000, should the budget be lower or higher? Are there any relationships between the goal and successful campaigns? 


### Analysis of Outcomes Based on Launch Date

The way to solve this case was thinking how to answer the questions above, especifically. When is the best time to launch a campaign? How to get a relation between the launch_at and the outcomes. It was required to display the months and see how many projects were successful, failed or canceled over the time, particularly over the years. 

To compare how the months were distributed over the years, the next table and chart: 


<img width="1205" alt="Screen Shot 2022-07-21 at 1 17 43 PM" src="https://user-images.githubusercontent.com/1729991/180308205-2d2e4cfc-5571-4c0e-b51f-e0315fdcad93.png">

- The pivot table shows a pinpoint in May that represents the month where the campaigns have overcome most successfully over the years.

- The pivot chart image "Theater Outcomes Based on Launch Date" shows a Line Chart with several pinpoints one of them represents the most successful month to launch a category that is May with 111 over 166 campaigns, the worst month to launch a campaign is in December where the amount of successful campaigns was 35 over 75 campaigns.


### Analysis of Outcomes Based on Goals


Some questions were answered. Is it a strategic decision to create a crowdfunding with that particular budget $10.000?, should the budget be lower or higher? Are there any relationships between the budget and successful campaigns? 

Displaying the outcomes (successful, failed, canceled) with the goal ranges or budget ranges. This helped to understand how many projects were successful with every range of budget. For example, with a budget between $10.000  and $14.999 there were 39 successful projects over 72. To have a most readable result we took the percentage. 

Then, with a budget between $10.000 to $14999 the percentage of successfulness is around 54% and the failness 46%. Is it the best budget for the project? 
To answer these questions, a table was designed with the range of possible Goals or budgets and the amount of the successful, failed, canceled projects and their percentages. 


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
