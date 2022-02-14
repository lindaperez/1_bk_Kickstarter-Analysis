# An Analysis of Kickstarter Campaigns

## Overview of Project
### Purpose

The project consist in analyze a dataset to generate insights. Based on a excel of Crowdfunding campaigns data with 4113 rows, determine the specific factors that influence the creation of a Play campain with an estimated budget of $10.000. Most specifically, generate sheets that serves as a tool to answer a decisive variety of questions for the creation of a crowdfunding campaign.


## Analysis and Challenges

Before to start developing a solution, it is important to think about possible questions that should be answer. These questions generally come up during the analysis of the project, the requirements and the raw data:

1. When is the best time to lauch the Play campaign? 

2. Is it an strategic decision to create a crowdfunding with that particular budget $10.000, should the budget be less or more? Are there any relationship between the goal and successful campaigns? 




### Analysis of Outcomes Based on Launch Date

The way to solve this case is thinking how to answer the questions above, especifically. When is the best time to launch the Play campaign? We inmediatly thought about, how to get a relation between the launch_at and the outcomes. We were able to think that we needed to display the months and see how many projects were successful, failed or canceled over the years.
After it, we could think about that filter by the parent category was very helpful to have a more acurate answer.

The way that this view answer this questions and some others is through a pivot table and a pivot chart. 

* The pivot table shows a pinpoint in May that represent the month where the Play campaigns have overcomed most successfully over the years. 


The best way to compare how the months were distributed over the years is the pivot chart.

* The pivot chart image "Theater Outcomes Based on Launch Date" shows a Line Chart with several pinpoints one of them represents the most succefull month to launch a category that is May with 111 over 166, some others worst escenarios like december where the amount of sucessfull campaign is very short around 35 over 75.

The process to solve it was following the steps in the Excel Module, here some images:

	1. StarterBook.xlsx Renamed.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/renamed.png)

	2. Resources folder created.
	3. Year column created.
	4. Date created conversion created.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/yearsFormula.png)


	5. Pivot table created.
	6. "Theater Outcomes by Launch Date." name setted
	7. Filters  "Parent Category" and "Years." created
	8. Placed the pivot table.
	9. Column filtered. 
	10. The pivot table looked as expected. 

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/9pivotTable.png)


	11. Filter by "Theater" created.
	12. Sort the campaign made.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/descendingOrder.png)

	13. Pivot table correctly.

	14. Image of the final pivot table.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/pivotTable.png)

	15. Chart created with the tittle Theater_Outcomes_vs_Launch.png

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)




### Analysis of Outcomes Based on Goals


For this case, we thought about the next question that was. Is it an strategic decision to create a crowdfunding with that particular budget $10.000, should the budget be less or more? Are there any relationship between the budget and successful campaigns? 
Initially the proccess to solve it was following the steps in the Excel module, but during the process we could realize that we were getting the answer, displaying the outcomes (successful, failed, canceled) with the the goal ranges or budget ranges. This helps to understand how many projects were successfull with every range of budget. For example, with a budget between $10.000  and $14.999 there were 39 successful projects over 72. To have a most readible result we took the percetage. Then, with a budget between $10.000 to $14999 the percetage of sucefulness is around 54% and the failness 46%. It it the best budget for the project? 

To answer this questions It was designed a table with the range of possible Goals or bugets and the amount of the successful, failed, canceled projects and their percentages. 

The countIf function helped to count the outcomes by some criterias.

The process to solve it was following the steps in the Excel Module, here the steps:

	1. Sheet "Outcomes Based on Goals." created.
	2. Columns setted.
	3. Ranges setted.
	4. COUNTIFS() function

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/countIf.png)

	5. Totals populated.
	6. Percentages calculated.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/1wholeView.png)
	
	7. Chart created.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)


### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	
	The view "Analysis of Outcomes Based on Launch Date" provides the way to answer our first fundamental question that is, What is the best time to create a "Play" Crowdfunding campaign based on the Parent category "Theater" over the years from 2009 and 2017. 

	May is the best month to launch a Play campaign. After this, the second one would be between April, May and somedays of June. After May the amount of outcomes start falling until January of the next year where they start increasing again. 

	

- What can you conclude about the Outcomes based on Goals?
	
	The view Analysis of Outcomes Based on Goals provides the way to answer our second fundamental question that is, Will the campaign be able to reach the goal expected, $ 10.000? 

	Having a budget of $10000 is hard to get with 54% of the cases aproved.

	The projects with a budget less than $1000 are the most successful with a 76% of acertiveness over the years. After it, could be a better idea reduce the budget to a range between $1000 to $4999 due to 73% of those projects got the whole budget. If the customer can not reduce the budget, something that can help is to have a greater budget, between 35000 and 44999, those projects were succefull in 67% of the cases.

- What are some limitations of this dataset?

	* Manipulating data is difficult because always we have the risk to change a value without noticing.
	* Apply a formula several times is something repetitive that could be done with a macro, reducing in this way possible errors.
	* There is not much information about some columns like spotlight or staff_pick, that can give more information to correlate it with the outcomes. 
	* There is not much information about the quality of the data, we guess is consistent. 

- What are some other possible tables and/or graphs that we could create?

We can ask more question to try to unhide more patterns to create a successful campaigns

	1. Create the campaign in a different country may help funding the goal budget?
		We can create a table with outcomes and countries and determine what is the country with the most succesful projects by "Play" subcategory.

![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Outcomes_by_Country.png)


	2. How long should be the campaign? 
		We can create a column with the number of days that every campaign last and create a table with the average of days that every campaign had, filtered by subcategory "Plays"  
		Then, we can see that the average days for the most succeful campaigns is 28.5days, with 412 succeful projects.
![This is an image](https://github.com/lindaperez/kickstarter-analysis/blob/main/Resources/Size_by_Outcomes_Country.png)



