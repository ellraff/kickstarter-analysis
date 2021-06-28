# Kickstarting with Excel

## Overview of Project
The goal of this project was to analyze kickstarter data to guide a hypothetical client named Louise.  The first step was to organize the data for the information relating to Louise's goal: to fund a musical called Fever in Great Britain.  This process included filtering and reorganizing the data we needed into  seperate sheets and creating pivot tables to get a better look at overal trends so we could advise whether her funding goal amount of 4,000 pounds would be acheivable compared to other projects like hers. Unfortunately, the data for Great Britain musical plays showed that the third quartile of pledges didn't even reach 2,000 and the max amount was closer to 3,000.  Therefor,  Louise would have a much higher chance of reaching a goal of 2,000 pounds.  The hypothetical goal was close to met very quickly but more data could be analyzed to predict the projects success.
### Purpose
The purpose of the next stage of analysis was to look closer at the launch dates of the kickstarter fundraiser to see what the effect that time of year had on the success of other campaigns. Another important goal was to analyze the outcome of the campaigns based on goals specifically with plays.  The intent of these analyses was to gice the hypothetical client a clearer understanding of what the duration and success rate would be based on her criteria.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the outcomes based on launch date, a pivot table was built with year and Parent Category as filters.  In the parent category filter, theater was selected to use outcomes relevant to Louise's campaign.   Outcomes were selected to fill columns and the rows were the months of the year.  Only successful, failed and canceled outcomes were used.  The pivot table displayed the count of each of the outcomes for each month of the year.  A pivot chart was created using these values to easily view the trends of the data displaying the outcomes based on launch date.  
![Outcomes vs. Launch Table](/resources/Outcomes_vs_Launch_PivotTable.png)

### Analysis of Outcomes Based on Goals
In order to visualize the outcomes based on goals trends, 
the count of successful, failed and canceled campaigns were collected based on ranges of goal amounts. The data used was based only on plays. The range started with $0 to $1,000, then $1,000 to $4,999 and up from there by increments of $5,000 up to $50,000.  $50,000 and up was the last bin.  Then, using the counts for each outcome in each range, percentages of each outcome compared to the total in that range were calculated and charted.  
![Outcomes vs. Goals table](/resources/Outcomes_vs_Goals_table.png)


### Challenges and Difficulties Encountered
I didn't perconally encounter any challenges, but I could understand how using countif statements to filter the data for the counts in each ange would be difficult to figure out at first.  I know it was a bit time consuming and required more repitition  then I typically like to use in coding.  I also had a strange experience with the main kickstarter data where it suddenly stopped allowing me to scroll down.  I could search for things but ti wouldn't move me to the position on the dataset. all the other worksheets were fine.  With a little research, I found out that excel can glitch like that from time to time but I had already used it for other worksheets.  In order to be able to look at my data better, I created a kickstarter2 dataset to use for the remainder of my calculations.  If seeing the second dataset in my files is confusing, that is why.

## Results

- ***What are two conclusions you can draw about the Outcomes based on Launch Date?***   
First of all, the summer months, primarily May, have the most successful outcomes.   Failed outcomes trend slightly up with the successful but the number of successful campaigns peaks at 100% more than failed in the May whereas the rest of the year is a much lower percentage.  There are 2 other peaks in February and October but February's peak is slight and shortlived.  The october peak is very slight for successful campaigns but jumps more durastically for failed campaigns so that may not be a good time.    
![Outcomes vs. Launch Chart](/resources/Theater_Outcomes_vs_Launch.png)

- ***What can you conclude about the Outcomes based on Goals?***   
It appears that the lower the goal, the higher chance there is of success.  Although the chart may suggest that higher goals can also be successful, in regards to the $25,000 to $49,999 range, the percentages are based on very scarce data compared to the lower amounts.  The total number of campaigns above $20,000 is 62, whereas the $1,000 to $4,999 range has 533 campaigns alone.  This implies that the data above $20,000 may be skewed due to relatively small sample sizes for each range.  But the clearest conclusing is that the highest rate of success lies below $5,000.  
![Outcomes vs. Goals Chart](/resources/Outcomes_vs_Goals.png)

- ***What are some limitations of this dataset?***   
As I mentioned above, the data includes a lot of outliers that can through off some calculations.  A larger sample size may assist with this or the awareness of this fact can be used to ensure percentages aren't weighed too heavily without looking closer at the data. Also, some of the campaigns ahve very high average donations which could mean that there are few very hgih donations that throw off the averages.  It may have been more helpful to have the median donations to see trends, but there is no access to that kind of data and unless it was reported, it would take a lot more work to find those values.

- ***What are some other possible tables and/or graphs that we could create?***   
It would be beneficial to make a graph of campaign duration based on goals.  Looking at this analysis alongside the other two could give us a clearer idea of what Louise may expect based on when she launched and what her goal was.

