# Kickstarting with Excel

## Overview of Project

### Purpose
using Excel formula and Pivot table to analyze outcomes of campaign and fundraising based on goals and Theater.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
In order to analyze the outcomes based on Launch date, I have Renamed column N Parent Category. have used " text to columns " option to created column O and name it Subcategory. I had to convert the unix time that is in column J to date time using the formula =(((j2/60)/60)/24)+Date(1970,1,1).
create column P and name it "Date Created conversion" and used the conversion time formula in it.
Creat column Q and name it Years based on column P which is "Date Created Conversion". have used formula "years" in column Q. 
Created Pivot Table and Chart Pivot and they are filtered by outcomes, parent category, date craeted and years. 
parent category and years were listed under filters
parent category filtered by Theater
years filtered by all 
outcomes was listed under columns 
date created was listed under rows
count of parent category was listed under values. 

### Analysis of Outcomes Based on Goals
in order to analyze the outcomes based on goals, I have craeted a new sheet named outcomes based on coals and used the goal's range that was provided to use to create a new table of 12 rows and 8 columns. 
have used COUNTIFS formula to generate the data in the successful, failed and canceled columns. I had to use 3 different criterias in this formula which is the outcome, goals and category.
 I have use a formula compining 3 cells to get the total projects in column E
 have used a formula to divide the successful, failed and canceled by the total projects to get the percentage for each category.
then I have made a Pivot and line chart filtered by Goal, percentage successful, percentage failed and percentage canceled. 
on the Pivot Column A I had to remove " less than 1000" to the top by selecting manual sort. 

### Challenges and Difficulties Encountered
getting the COUNTIFS formula correct for each category. after using the formula in a cell I had to subtract the result from the cell above it to get the correct number and doing it for each formula.   

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
in May , June and July were the most successful Campaign.
in May , July and October were the most failed campaign. 

- What can you conclude about the Outcomes based on Goals?
the most successful campaign was the one with goels less than the 1000
the most failed one was with goals between 45000 and 49999.
there was no canceled compaign  

- What are some limitations of this dataset?
the deadline and the launched dates are in unix format

- What are some other possible tables and/or graphs that we could create?
outcomes based on currency, this way we would know the cheapest campaign after changing the currency to dollars. 
