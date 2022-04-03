# An Analysis of Kickstarter Campaigns

## Overview of Project
At the beginning, we were introduced to Louise, an up-and-coming playwriter who wanted to start a crowdfunding campaign on Kickstarter to help fund her play, *Fever*. She estimated a budget of over $10,000 and was hesitate in jumping into her first fundraising campaign and reached out for some helpful insights. She was hoping my analysis can discover if there are any specific factors that makes a similar project's campaign successful and if so, we would be able to set her campaign to mirror other successful ones in the same category. Once that was completed, she requested this following project:

Louise proceeded with her crowd fundraiser after the initial review and *Fever* is already close to its fundraising goal in a short amount of time. But now she would like me to look specifically into how different campaigns fared in relation to their launch dates and their funding goals.

### Purpose
The purpose of this project is to review and visualize specifically from the Kickstarter dataset two separate relationships. The first one is regarding the final outcomes based on their launch month for the theater parent category. The second one is final outcomes based by their preselected goals specifically for the plays subcategory. The requested deliverables to be provided to Louise are:

- [x] Deliverable 1: Outcomes Based on Launch Date Chart
- [x] Deliverable 2: Outcomes Based on Goals Chart
- [x] Deliverable 3: Analysis of the Results

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To complete the first deliverable, I created a pivot table to create a graph *image below* visualizing the campaign outcomes (successful, failed, and canceled) based on launch dates. From the Kickstarter dataset I worked on previously, I created a new coloumn for the Years. Then utilizing the the Year function to extract the years, I created a pivot table to illustrate the parent category Theater by months of the year and sorted in descending order. From there, I created a line chart from the pivot table to visualize the relationship between outcomes and launch month.
![Outcomes Based on Launch Date Image](/01-Kickstarter/Resources/Theater_Outcomes_vs_Launch.png)


### Analysis of Outcomes Based on Goals
To complete the second deliverable focused on Plays category, I created a new sheet with the following columns (goal, number successful, number failed, number canceled, total projects, percentage successful, percentage failed, and percentage canceled). The goal column was grouped into 12 groups from min of less than $1,000 to $50,000+ and $5,000 increments in-between. This analysis relied on using the COUNTIFS to populate the number successful, number failed, and number canceled. Then using the SUM function to add the rows together to complete the final columns of percentages. From there, I created a line chart with the goal-amount ranges on the x-axis, the percentage of successful, failed, or canceled projects on the y-axis to visualize the outcomes based on goals. *image below*
![Outcomes Based on Goals Image](/01-Kickstarter/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
- I heavily referenced to the COUNTSIF() video that was included in the hint to assist me with creating the table that built the Outcomes Based on Goal. I was very glad that a checks and balance method was included so that I could check my work as well before going
- Initially, my graph for the Outcomes Based on Goals was not in the correct order to correctly depict the relationship because two of the rows has text with the numbers "Less Than 1000" and "50000 or More" so using the option for ascending or descending did not solve this problem. I was able to search and find a guide regarding different sorting options in a pivot table that was to illustrate how to achieve it without losing the data. 
- From an aesthetics standpoint, I realized prior to pulling the screenshots that there were field buttons on the graphs and I searched and found how to remove all the field buttons so they will not take away from the visuals and the information they are portraying. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    - The positive take away is that the month of May is the busiest time of the year with 166 total campaigns but also has yield the greatest number of successful theater campaigns (111) and highest number of successful rates as well (67%). So the middle of the year is the most ideal time to launch the campaign.
    - The negative take away is that the last month of the year and first month of the year has a history of yielding the highest percentage of failed campaigns (47%) and the highest number of canceled campaigns (7) respectively. So it would be best to avoid launching a campaign either at the beginning or end of the year. 

- What can you conclude about the Outcomes based on Goals?
    - To have a lower goal amount up to $4,999, your chance of success is much higher based on previous data (above 70%) representing 720 projects. The higher goal amounts do show a higher percentage of failure but the data is very limited with the collective total projects (42) above $25,000 

- What are some limitations of this dataset?
    - Depending on which parent category or subcategory that is of interest, there is a lack of strong data to support a convincing analysis. 
    - The data only has a historical timeline of nine years so some trends cannot be forecasted. 
    - The amount of data provided per country can be limited. 

- What are some other possible tables and/or graphs that we could create?
    - A graph to see the relationship between the average donations in similar category would be able to help give insight on the donation benchmarks to use in the future and see how closely it may or may not align with Louise's current protectory. 
    - A table to show the relationship between the number of days between the launched date and end date and the outcomes to depict if possibly there is any relationship between if it's better to go for a shorter campaign to entice the pressure of now or never or for a longer campaign for a possibility of higher exposure rate. 