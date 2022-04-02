# An Analysis of Kickstarter Campaigns

## Overview of Project
At the beginning, we were introduced to Louise, an up and coming playwriter who wanted to start a crowdfunding campaign to help fund her play, Fever. She estimated a budget of over $10,000 and was hesitate in jumping into her first fundraising campaign and reached out for some helpful insights. She is hoping my analysis can discover if there are specific factors that makes a project's campaign successful and if so, we would be able to set her campaign to mirror other successful ones in the same categroy.

She proceeded with her crowdfundraiser and Fever is already close to its fundraising goal in a short amount of time. But now she would like me to look specifically into how different campaigns fared in relation to their launch dates and their funding goals.

### Purpose
The purpose for this project is to review specifically from the Kickstarter dataset two seperate relationships. The first one is regarding the outcomes of if it was successful, failed, or canceled by their launch month for the theater parent category. The second one is outcomes of if it was successful, failed, or canceled by their preselected goals sepecfically for the plays subcategory.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
![Outcomes Based on Launch Date Image](/01-Kickstarter/Resources/Theater_Outcomes_vs_Launch.png)
### Analysis of Outcomes Based on Goals
![Outcomes Based on Goals Image](/01-Kickstarter/Resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
- I heavily referenced to the COUNTSIF() video that was included in the hint to assist me with creating the table that built the Outcomes Based on Goal. I was very glad that a checks and balance method was included so that I could check my work as well before going
- Initally, my graph for the Outcomes Based on Goals was not in the correct order to correctly depict the relationship because two of the rows has text with the numbers "Less Than 1000" and "50000 or More" so using the option for ascending or descending did not solve this problem. I was able to search and find a guide regarding different sorting options in a pivot table that was to illustrate how to achieve it without losing the data. 
- From an astestics standpoint, I realized prior to pulling the screenshots that there were field buttons on the graphs and I searched and found how to remove all the field buttons so they will not take away from the visuals and the information they are protraying. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
    - The positive take away is that the month of May is the busiest time of the year but also has yield the most number of successful theater campaigns and highest number of successful rate as well. So the middle of the year is the most ideal time to launch the campaign.
    - The negative take away is that the last month of the year and first month of the year has a history of yielding the highest percentage of failed campaigns and the highest number of canceled campaigns respectively. So it would be best to avoid launching a campaign either at the beginning or end of the year. 

- What can you conclude about the Outcomes based on Goals?
    - No matter how high or low the goal is set for the campaign, it can still fail. There is no consistent benchmark that would ensure you would be able to meet your goal as long as it is x. 

- What are some limitations of this dataset?
    - Depending on which parent category or subcategory that is of interest, there is a lack of strong data to support a convincing analysis. 
    - The data only has a historical timeline of nine years so some trends cannot be forecasted. 
    - The amount of data provided per country can be limited. 

- What are some other possible tables and/or graphs that we could create?
    - A graph to see the relationship between the average donations in similar category would be able to help give insight on the donation benchmarks to use in the future and see how closely it may or may not align with Louise's current projectory. 
    - A table to show the relationship between the number of days between the launched date and end date and the outcomes to depict if possibly there is any relationship between if it's better to go for a shorter campaign to entice the pressure of now or never or for a longer campaign for a possibility of higher exposure rate. 