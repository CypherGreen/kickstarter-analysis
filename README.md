# **Kickstarting with Excel**
## **Overview of Project**
*Performing analysis on Kickstarter data to uncover trends*
---
### **Background of Project**
The purpose of this project was to assist Louise in analysing Kickstarter data to look for trends that would help her with her own Kickstarter campaign. She had a goal of $12,000 to raise and getting to look through historical data outcomes from other similar projects helped to make crucial decisions for her theater play's success.
---
## **Analysis and Challenges**
The initial dataset contained over 4,000 rows of Kickstarter data, so the first course of action was to look at what kind of data there was and decide the best conversion of it so Louise could view it more easily. Some of the columns had to be re-formatted into the correct structure before any analyses could be pulled from them. Through filtering the data and using conditional formatting, key notes could be made regarding the timeline of a project's success rate, the average amount of a successful campaign's fundraising goal, and most importantly, whether a theater campaign in the U.S. would be successful. The initial dataset was too large to conduct any beneficial analysis so organizing the most important columns and pulling what was needed into seperate worksheets assisted the analysis and saved time since the initial raw data was no longer needed by the end of our analysis.
---
### **Analysis of Outcomes Based on Launch Date**
Creating a pivot chart for the Kickstarter outcomes helped to show the success rate of these campaigns throughout the year. This chart allowed a quick and easy glance at detecting the greatest chance of success through the most successful months. The time of year when a Kickstarter begins had a significant effect on a project's outcome. Theater plays in the U.S. seem to do fairly well and have a good possibility of succeeding.
![Thtr_Otcms_vs_Lnch](https://github.com/CypherGreen/kickstarter-analysis/blob/master/Thtr_Otcms_vs_Lnch.png)

### **Analysis of Outcomes Based on Goals**
The percentage of successful versus failed projects can be viewed in a different perspective when filtering by the ranges of goal amounts. The Outcomes Based on Goals chart shows that most of the failed campaigns had an extremely high fundraising goal that was way above the average Kickstarter goal amount. This will help Louise in determining how much money to set for her goal amount that will be reasonably achieveable. 
![Otcms_vs_Gls](https://github.com/CypherGreen/kickstarter-analysis/blob/master/Otcms_vs_Gls.png)

### **Challenges and Difficulties Encountered**
The challenges encountered throughout out this analysis were:
1. Having to use the IFERROR formula to nest two formulas to fix the division error in the Average Donation column created from the Pledged and Backers columns.
2. When trying to use the correct date conversion formula, the only way to use it was to not change J2 to the first cell of the Deadline column, but keeping J2 in the formula let it run smoothly throughout the column. When trying to replace J2, an error showed and would not let the formula calculate correctly.
3. When trying to use the formulas for the average, median, and standard deviations on the Descriptives Statistics worksheet, the workbook would not let the formulas run correctly even though the formula was correct. Going back to the main Kickstarter worksheet and highlighting the whole columns for both Goals and Pledges showed a correct average calculation at the bottom of the worksheet that Excel automates. Having a Learning Assistant check it over also was unsuccessful in determining how the error came about. They suggested the error was due to calculation of the formula switches over to manual instead of automatic, however, that turned out not to be the case. Unable to determine the cause of this bug in the workbook, the best solution at this point was to type out the desired formulas into a seperate workbook then copy and paste the results (along with the formulas used) back into my original workbook. This solved the issue.
---
## **Results**
For the final summary of this analysis, a couple of important decisions can be made regarding Louise's theater play campaign. First, based on what we can see from the Outcomes Based on Launch Date, she will need to plan her launch date for the month of May to have the best chance of meeting her goal. Our chart also implies that starting a campaign later on in the year will significantly decrease the possibility of her campaign succeeding. Secondly, the chart Outcomes Based on Goals clearly shows the necessity in having a goal amount that does not overexceed the average Kickstarter goal amount. Louise may have a hard time succeeding with her initial $12,000 goal amount, since it is higher than the average. Readjusting her goal will give her project a much better chance of succeeding.

Some limitations of this dataset could include the following:
1. Plays in the U.S. can be viewed and analysed as a whole, however, it would be even better to have a more specific analysis of the campaigns being funded closer to where Louise expects to develop her project. Location can be important in determining if the population where she expects to do business at could be enticed with promotions such as physical ads. Targeting where to pull the most ad revenue would be the easiest and fasted way to target her key consumers.
2. Since what our current dataset shows what right now is a broader overview, having another chart that only looks at theater plays within the past year would be beneficial to look at to see what the popularity currently reveals. Perhaps even analysing by play genre would benefit Louise as well.
