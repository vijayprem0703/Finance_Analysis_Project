# Personal Finance PowerBI Dashboard

A project that utilizes Microsoft PowerBI to analyze personal financial data and visualize expenses through an interactive dashboard.


## Problem Description

As one should, I have been keeping track of all my daily spending using Microsoft Excel. Using basic sorting/filtering in Excel I'm able to see a very high-level overview of my spending. In order to perform data analysis at a more deeper level, we will turn my static Excel data into dynamic PowerBI dashboards.


## Project Goals

Here are the questions I would like the PowerBI dashboards to answer:
- Monthly spending (in a given year).
- How much money spent per item category.
- List all expenses with comments.
- How much money spent per location.
- The number of purchases in various price ranges.
- Quarterly and weekly spending information.
- Various average costs (per week, month, day).
- Comparison of food costs to restaurant costs.
- Spending behavior when I'm sick.
- Comparison of weekday and weekend spending.

In order to answer these questions, I invested time in planning the PowerBI measures I would need to create and also planned a rough outline of the dashboard visuals I wanted. 


## Data Analysis Summary

Here are the dashboards that I created. If you would like to actually play around with these dashboards see the end of this readme for instructions:

![alt text][ExecSumm]

![alt text][Granular]


## Hardware and Software Used

- Python
- Python Libraries: openpyxl, os
- Windows 10 Machine
- Microsoft PowerBI Desktop
- Microsoft Excel
 



## Data Collection Methodology

I collected this data by keeping all purchase receipts and inputting the data manually into Excel. The information I kept track of was: Date, Item Category, Price, Location, Comment.

In order to import this data into PowerBI, it was quite the process. Since the data was contained in *multiple Excel sheets in the same Excel workbook*, I first had to separate the sheets into their own Excel workbook - this turned out to be the easiest avenue to importing the data.


## Data Cleaning

There was quite a bit of data cleaning to do. I had to do some basic editing of the 'Item' category column, in order to have consistent categories. For example, I had 'hair cut', 'Hair cut', 'Hair-Cut' as separate categores, and so had to standardize this into simply a 'Hair Cut' category.

There was a lot of work needed to be done with dates. Some dates were of a 'Text' type, some were a 'General' type, and still others were the 'Date' type. These had to be standardized.

Finally, only a few rows contained null entries, so I simply chose to remove these rows from the overall dataset; This would not drastically affect the variance of the overall data.


## Conclusion

Using PowerBI I was able to visualize my purchases data in an interactive way. This allowed me to drill deeper into my spending behaviour and with this information I can now be more conscientious of what I choose to spend my money on.


## Future Steps

For future improvement, we can consider the following ideas:
- Attempt to create more visually appealing dashboards (perhaps you can find a template to use?).
- Perhaps there is a way to generalize this dashboard so anyone can use it? (Launch via Docker container?)
  - Would need to ask users to standardize their Excel sheets a certain way?
- Think of new informative metrics that may be useful.
- Create new or modify existing dashboards for ease-of-use on mobile/tablet devices. (Can be done in Power BI Desktop)
<!-- Image References -->

[ExecSumm]: images/executive_summary.png "Main summary of data"
[Granular]: images/granular_info.png "Second dashboard for detailed inormation"
[DashPlan]: images/dashboard_planning.jpg "My original layout for the dashboards"
[Questions]: images/investigative_questions.jpg "The original questions I wanted answers to"
