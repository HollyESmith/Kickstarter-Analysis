# Kickstarting with Excel
Performed analysis on Kickstarter data to uncover trends
## Overview of the Project
Louise asked how different theater play campaigns fared in relation to launch dates and funding goals. 
### Purpose
Analyze success/failure rates and launch date data to determine the best time to launch a campaign, and analyze goal data to propose a reasonable budget goal for Louise. 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
First, I wanted to determine what month most successful Kickstarter theater campaigns were launched. Using the given Kickstarter data, I created a pivot table to show how many campaigns were successful, failed and canceled by month, then filtered the table to show only theater campaigns. Then I created a Pivot Chart to visualize the results: 
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/97558998/154856656-22136404-8702-4ab4-ab2b-02376dc4c88d.png)
### Analysis of Outcomes Based on Goals
Next, I wanted to determine the number of successful, failed, and canceled theater campaigns based on monetary goals. I created a table of defined dollar-amount ranges and calculated the percentage of successful, failed and canceled theater projects. Then I created a chart to visualize the results:
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/97558998/154857007-c989ebcd-3d7e-4cb7-b5d5-c2871799c18b.png)
### Challenges and Difficulties Encountered
1.	I struggled with figuring out how to sort outcomes in descending error. I googled different ways to ask the question and finally found the answer here: https://support.microsoft.com/en-us/office/design-the-layout-and-format-of-a-pivottable-a9600265-95bf-4900-868e-641133c05a80#:~:text=In%20the%20PivotTable%2C%20right%2Dclick,bottom%20border%20of%20the%20cell.
2.	Minor issues with using Excel on MacOS. I have a lot of Excel experience on the PC I that used at work, but at home I have a Mac and had some difficulty finding commands. For example, how to change the color of lines in the line graph. Easily solved with a Google search.
3.	When verifying the Outcomes Based on Goals data, I discovered that I was one short on the number of successful projects (total should have been 694 but I had 693). I reviewed my formulae and verified that there were no blank cells that would not have been counted. Then I narrowed down the location of the error by sorting the Kickstarter data by Goal amount and counting each range. I determined that the error was in the 1000-4999 group and quickly discovered that there was only one value of 4999. I re-checked the formula to discover that instead of “<=4999” I had typed “<4999,” omitting the “=” which I didn’t catch when I initially reviewed the formulae.
## Results
- Conclusions drawn about the Outcomes based on Launch Date:
  1. The most successful month to launch a theater campaign is May, followed by June, despite the large number of theater projects that are launched during those months.
  2. The success rate falls steadily from its peak in May; strong recommendation to avoid launching a theater project in the 4th quarter of the calendar year (October/ November/ December).
- Conclusion drawn about the Outcomes based on Goals: There is a higher likelihood of success when the goal is <$5,000; the percentage of successful projects with a goal of <$1,000 being slightly more successful (76%) that those with a goal of $1,000 - $4,999 (73%). I conclude that success is strongly linked to modest goals, presumably because it’s easier to meet a smaller monetary goal. However, projects with goals between $35,000 and $45,999 had a success rate of 67%, though there were far fewer of these projects (9) than projects less than $5,000 (720), indicating that the success of the projects is not entirely dependent on its monetary goal. In regard to Louise’s current budget of $10,000 for her Fever production: similar campaigns in this goal range had a 54% success rate.
- Dataset Limitations: We looked at the number of theater play campaigns that were successful by month, and the amount of goal that was most probable for success. However, we didn’t look at the relationship between the month of launch and amount of goal. For example, I would like to know what month(s) the 6 successful campaigns with the larger budgets (%35,000 - $44,999) were launched.
- Other possible tables/graphs that we could create: A dual-axis combination graph may lend itself to analyzing relationships between disparate data.
