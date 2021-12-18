# Kickstarting with Excel

## Overview of the Project - [Kickstarter Challenge Excel File](https://github.com/AmairaniR/kickstarter-analysis/blob/main/kickstarter_challenge.xlsx)

### Purpose

This Excel Workbook analyses the theatre outcomes by launch date and the outcomes based on goals of various Kickstarter campaigns to help the client Louise determine what month of the year is best for launching a campaign and what goal range is mostly likely to lead to a successful campaign. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

For my first analysis, I first had to create new column in the “Kickstarter” worksheet titled, Years, in order to extract the year from the Date Created Conversion column. I could then perform my analysis of the sheet titled “Theatre Outcomes by Launch Date” by creating a pivot table from the dataset on the “Kickstarter” sheet. I then filtered it by ‘Parent Category’ and ‘Year’, I entered the ‘Date Created Conversion’ for the rows and removed the added ‘Years’ and ‘Quarter’ categories, and finally I moved ‘Outcomes’ into the values and columns fields to finish creating the pivot table. From there I created a line chart from the pivot table to make a visual representation of the relationship between launch dates and outcomes. 

[Image - Theatre Outcomes vs Launch Dates](Resources/Theater_Outcomes_vs_Launch.png.png)

### Analysis of Outcomes Based on Goals

For the second analysis, I analyzed the outcomes of the Kickstarter campaigns based on the goals. I reduced the goals to specific ranges and created individual columns for successful, failed, and canceled campaigns. I then used a =COUNTIFS formula to filter and count for the number of plays within the goal range and for the specific outcome I was looking for. I then totaled the projects for each goal range and calculated the percentage for each outcome. With this new dataset I created a line chart of the percentages for each outcome. 

[Image - Outcomes Based on Goals](Resources/Outcomes_vs_Goals.png.png)

### Challenges and Difficulties Encountered

While performing this analysis I did not encounter many challenges. However, populating the second dataset with COUNTIFS formulas that needed to be changed for every cell became tedious and time consuming. While the changes to the formula only consisted of a few characters at most for every cell, this type of task would be much more time consuming and repetitive for a larger dataset.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

  1. Since May has the highest number of successful theatre campaign launches, it would be best for Louise to launch a theatre campaign in May.
  2. December has the lowest number of successful theatre campaign and an almost equal number of failed campaigns signifying that a campaign is just as likely to succeed as it is to fail during this month. However, the chance for success overall is lower than it is for all the other months and therefore not a good month to launch a campaign.

- What can you conclude about the Outcomes based on Goals?

  1. The conclusions for this dataset were not as clear, however, generally, successful campaigns had lowers goals, and failed campaigns had higher goals. Louise should probably keep her goal for any future plays under $2000 where the numbers are more predictable.

- What are some limitations of this dataset?

Some limitations for this dataset is that there is no information for the total duration of the campaign. It would also be more informative if there was a timeline for when exactly the goal was met for successful campaigns. 

- What are some other possible tables and/or graphs that we could create?

I think it would be interesting to do an analysis of Outcomes based on the duration of the campaign by using the Date Created Conversion column and the Date Ended Conversion column to see whether longer or shorter campaigns effect the outcome. Once this information is extracted, it would also be interesting to see how much more money is raised with campaigns that last longer. 
