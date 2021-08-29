# Kickstarting with Excel

## Overview of Project

### Purpose
- To perform data analysis on several thousand crowd-funding projects to discover trends and patterns.

- To visualize campaign outcomes under *"plays"* subcategory based on their **launch dates** and their **funding goals** using Kick-starter dataset for Louise.


## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

This Analysis helps one understand campaigns' performance in relation to their launch dates. It primarily focuses on campaigns under **Theater** category. 

By using *Pivot tables* from Kick-starter dataset we have presented "Launch Date Conversion" as Rows and "Outcomes" as columns with filters "Parent Category" and "Years" to show "Count of outcomes" as a metric. We then have used *Pivot Charts* to generate the Line Graph
for the created Pivot Table.The hyperlink and the image for the graphs are given below.

[https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png](https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png "Theater_Outcomes_vs_Launch")

![Theater_Outcomes_vs_Launch](https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

**Findings**

- May has highest number i.e. 111 of successful Kick-starter campaigns launched. February , April and August have second highest i.e. 71,71 and 72 respectively.

- May, June, July, August and October all had roughly the same number of failed campaigns launched, around 50. 

- December has lowest number of successful campaigns i.e.37. The number of Successful and Failed campaigns were nearly same in this month.

- October has 0 campaigns canceled.



### Analysis of Outcomes Based on Goals

This Analysis helps one understand campaigns' performance based of **specific goals range criteria** . For **"Successful","Failed","Canceled"** campaign outcomes we are adding the counts if the specified Goal criteria is met using **COUNTIFS()** function.
We then calculate the Total project outcome and then the percentage of each outcome over Total project outcome for all goal criteria. Next we generate the Line Graph with outcome percentages on Y axis and the Goal criteria on X axis. The hyperlink and the image for the graphs are given below.


[https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Outcomes_vs_Goals.png](https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Outcomes_vs_Goals.png "Outcomes_vs_Goals")

![Outcomes_vs_Goals](https://github.com/Sheetaltkr/Kickstarter-Analysis/blob/main/resources/Outcomes_vs_Goals.png)

**Findings**

- For goals lesser than $10000 we have highest percent of successful outcomes.76% being the highest success rate.

- For goals greater than $10000 we have highest percent of failed outcomes. 100% being the highest failure rate.

- 0 campaigns were canceled.


### Challenges and Difficulties Encountered

- Error was encountered for division by 0 operation while calculating the % canceled outcomes. This was handled using IFERROR() function.
- Writing code for Outcomes Based on Goals was tedious while hard-coding criteria values. Creating new table for criteria and then referencing those cells in the code helped with this problem. This will also help for any future modifications if goal criteria changes.
- The graphs plotted by applying filters could get distorted if the filters were removed or changed on the source kick-starter sheet. Using a separate worksheet with dataset of the filtered data could help to avoid this issue.
- The code for applying Range based Goal criteria along with multiple other criteria could be long. Use of correct count function COUNTIFS() instead of COUNTIF() is important for this analysis.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

	- Campaigns launched in May were most successful.
	- Campaigns launched in Dec were least successful. Holidays may have an impact.
	
- What can you conclude about the Outcomes based on Goals?
	
	- The lower the goal higher are the chances of success

- What are some limitations of this dataset?
	- This Dataset has live campaigns data which cannot be considered for analysis
	- The columns deadline and launch date are not in required formats had to be converted in standard long date format to show the day,month and year.
	- Category and subcategory are inside a single column delimited by "/". The data had to be separated to be useful for using category/subcategory for our analysis.

-  What are some other possible tables and/or graphs that we could create?
	We could create below tables and graphs
	- Additional Goal criteria for goal =50000 as part of Outcomes Based on Goals
	- Category/Subcategory and statistics (Bar graph)
	- Country and statistics (Bar graph)
	- Outcomes based on Year (Line chart)
	- Descriptive statistics (Box and whisker)
	- Project outcome and Duration of project statistics(Bar graph)
	- Additional graph for outcomes based on % of goals (Pie chart)
