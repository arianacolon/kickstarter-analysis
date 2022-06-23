# Kickstarting with Excel

## Overview of Project
Louise is an up and coming playwright who has come close to her fundraising goal, $10,000, for her play, Fever. To educate Louise on the correlation between different campaign outcomes and their launch dates and funding goals, data has been collected from previous crowdfunding campaigns to interpret and analyze. [Kickstarter_Challenge.xlsx](https://github.com/arianacolon/kickstarter-analysis/files/8963529/Kickstarter_Challenge.xlsx)

### Purpose
The purpose of this analysis is to see how launch dates and funding goals of crowdfunding campaigns similar to hers affect the outcomes of them.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To begin my analysis of outcomes based on the launch date, I created a PivotTable, in the Theater Outcomes by Launch Date worksheet, which was filtered by parent category and the years that the crowdfunding campaigns were created. I changed the parent category filter to only present day for “theater,” and kept the years filter to show all, from 2009-2017. The legend area and values area of the PivotChart are both represented by the outcome field. The legend area will inform us if the campaign was successful, failed, or canceled and the values areas informs us of the amount for each column. The date created conversion field is used in the axis area to help us identify the amount of successful, failed, and canceled campaigns for each month throughout all the years.  I then created a visualization, specifically a line graph with markers, to help display the trend how the values of the successful, failed, and canceled campaigns varied of the twelve months throughout the years. <img width="249" alt="Theater_Outcomes_vs_Launch" src="https://user-images.githubusercontent.com/107401667/175203801-49526c71-98b7-4a43-a834-84f4f5d81051.png">

### Analysis of Outcomes Based on Goals
To begin the analysis of outcomes based on goals, I created a second goal column in a new worksheet, called Outcomes Based on Goals, where each cell under this column identified different increment amounts of money for the goals of the crowdfunding campaigns. I then used the COUNTIFS function in Excel to determine how many crowdfunding campaigns met certain criteria. Column B is number of successful plays, Column C is number of failed plays, and Column D is number of canceled plays. I then calculated the number of total projects and used this to calculate the percentage of successful, failed, and canceled plays based on the range of the goal amount. Lastly, I created a visualization of a line graph to represent how the percentage of successful, failed, and canceled campaigns correlated to the different goal ranges. <img width="394" alt="Outcomes_vs_Goals" src="https://user-images.githubusercontent.com/107401667/175203848-4fccef49-7234-4af8-b228-d9d761e6e106.png">

### Challenges and Difficulties Encountered
The only challenge I encountered was with the COUNTIFS function. As I first applied the function to column B, my results showed all zeroes. I was confused at first because I knew that was not accurate based on the data provided from the Kickstarter worksheet. As I looked through the criteria I typed for the COUNTIFS function, I realized I put “subcategory” instead of “plays.” Once I corrected this, my data was fixed and displayed the correct results.

## Results
1. A conclusion I can draw about the Theater Outcomes by Launch Date is that February, May, or October are the best three suggested months to launch a theater campaign because they all represent peaks in the graph. Specifically, May would be the most ideal because it had the most successful outcomes with a value of 111. A second conclusion is launching a theater campaign in December is roughly a 50/50 chance of success or failure. In this month, there was 37 successful campaigns and 35 failed campaigns.
2. Based on the Outcomes based on Goals, I can conclude that the most successful play campaigns were the ones that were less than 1000 because it has the highest percentage.
3. A limitation of this dataset is using the Parent Category instead of the Subcategory in the PivotTable for Theater Outcomes by Launch Date. Using the Subcategory as a filter instead would have allowed me to view the launch dates of plays since that is what Louise is interested in and would have helped visualize data more specifically to her interest.
4. For the PivotTable in Theater Outcomes by Launch Date, a stacked bar graph could have been used to visualize instead of the line graph. The X-axis could have displayed the months and each month have a bar that is made up of the amounts of successful, failed, and canceled outcomes.
