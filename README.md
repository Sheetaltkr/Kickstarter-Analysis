# Kickstarting with Excel

## Overview of Project

### Purpose
- To perform data analysis on several thousand crowd-funding projects to discover trends and patters.

- To visualize campaign outcomes under *"plays"* subcategory based on their **launch dates** and their **funding goals** using Kick-starter dataset for Louise.


## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

This Analysis helps one understand campaigns' performance in relation to their launch dates. It primarily focuses on campaigns under **Theater** category. 

By using *Pivot tables* from Kick-starter dataset we have presented "Launch Date Conversion" as Rows and "Outcomes" as columns with filters "Parent Category" and "Years". We then have used *Pivot Charts* to generate the Line Graph
for the created Pivot Table.The hyperlink and the image for the graphs are given below.


####Findings

- May has highest number of successful Kick-starter campaigns launched . 

- January, June, July and October all had roughly the same number of failed campaigns launched.

- October has 0 campaigns canceled.

- December has lowest number of successful campaigns. Number of Successful and Failed campaigns nearly same in this month.



![Theater_Outcomes_vs_Launch](C:\Users\sheet\OneDrive\Documents\Berkley Bootcamp\Assignments\Kickstarter_Analysis\Module 1 Challenge\resources\Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals

This Analysis helps one understand campaigns' performance based of **specific goals range criteria** . For **"Successful","Failed","Canceled"** campaign outcomes we are adding the counts if the specified Goal criteria is met using **COUNTIFS()** function.
Then we calculate the Total projects and percentages of each project with given outcomes over Total projects. Next we generate the Line Graph for percentages on Y axis and the Goal criteria on X axis. 

####Findings

- May has highest number of successful Kick-starter campaigns launched . 

- January, June, July and October all had roughly the same number of failed campaigns launched.

- October has 0 campaigns canceled.

- December has lowest number of successful campaigns. Number of Successful and Failed campaigns nearly same in this month.

### Challenges and Difficulties Encountered



## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
