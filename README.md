# Kickstarting with Excel

## Overview of Project

My client is conducting a crowdfunding campaign to stage a play they have written. They requested I use my expertise with Excel to maximize their chance of success by analyzing similar crowdfunding campaigns and identfying factors that correlate with success. 

### Purpose

The purpose of this analysis is to maximize my client's chance of success in crowdfunding their play. I analyzed the data to identify factors that 1. correlate with a successful theater crowdfunding campaign and 2. are under my client's control.

## Analysis and Challenges

I was presented with a large dataset of over 4,000 Kickstarter campaigns from all over the world. I then narrowed the data to include only theater campaigns. I then looked for factors within my clients control that might influence the outcome of their fundraising campaign. I identified two: launch date and goal amount. I then created two separate tables for outcomes based on these factors. Finally, I created charts to visualize the data.

The dataset presented several challenges over the course of analysis. First, I needed to clean the data by converting dates to an understandible format as well as create new columns from existing columns so more data could be used in my analyses. Then, I needed to filter the data for relevant campaigns. I was able to accomplish all of this by using Excel's formulas, functions and other features.

### Analysis of Outcomes Based on Launch Date

Below is a chart showing the outcomes of theater Kickstarter campaigns based on launch date. 

![Outcomes by Launch Date](https://github.com/LiShanDa2021/kickstarter_challenge/blob/main/Theater_Outcomes_vs_Launch.png?raw=true)

We can see from the chart that success is the norm in theater crowdfunding campaigns with campaigns beginning in late-spring to mid-summer having the greatest chance of success. Outside of the summer theater season, February seems to be the best time to launch a theater fundraiser. According to the chart, the worst time to raise money for a theater production is December with November, January and September close behind.

### Analysis of Outcomes Based on Goals

The chart below displays the outcomes of crowdfunding campaings for plays by goal amount.

![Outcomes by Goal Amount](https://user-images.githubusercontent.com/87392984/133280623-9e96f32d-fac5-41e1-b2cc-38e3d3cfdcaf.png)

From the chart we can see that the plays with the greatest likelihood of success are those with goals of less than $1000. The rate of success remains fairly steady (dropping only slightly) up until $5000. After that point the rate of success drops sharply. Though the rate of success is relatively high at the $35000 to $40000 level, I would caution against drawing conclusions from those data points because the sample size at that range is small as you can see from the table below.

![Outcomes by Goal Data](https://user-images.githubusercontent.com/87392984/133281053-7224b4e0-fada-467f-844c-780d0ccdd6ee.png)

### Challenges and Difficulties Encountered

I encountered challenges immediately upon opening the .xlsx file containing the data set. First of all, the data needed cleaning. Some of it was not in a format that was not user-friendly. For example, the dates were in time stamp format. To correct this I applied a formula to convert time stamps into dates as displayed in the image below.

![Date Conversion Formula](https://github.com/LiShanDa2021/kickstarter_challenge/blob/main/Screen%20Shot%202021-09-12%20at%206.44.24%20PM.png?raw=true)

Other data was in an understandable format but needed to be separated to be more useful. My client is staging a play, but the theater category encompassed more than just plays. It also included musicals and theater spaces. Clearly, staging a production is different than opening a theater space. I needed to separate the theater data into subcategories. Fortunately, the category column contained the subcategory information. Unfortunately, the subcategories were contained within the category column. It was difficult to sort by plays if it was contained in the theater category. Fortunately, I was able to use Excel's text to columns feature to separate the subcategory from the category. Finally, in order to analyze the chances of success based on a given factor, I needed to find the number of successes, failures and cancelations in a given category. This was not included in the dataset. Fortunately, I was able to use Excel's `COUNTIF function to create a table with these numbers.

Then, there was the shear size of the dataset to contend with and mountain of irrelevant data it contained. There were over 4000 entries and most of them were not for theater campaigns. I was able to circumvent this easily by creating pivot tables and filtering for theater campaigns.


## Results

### Conclusions Based on Analyses
In conclusion, I analyzed the outcomes of theater kickstarter campaigns based on two factors: launch date and goal amount. From the analysis based on launch date, I conclude that the best months to launch a kickstarter campaing for theater are May annd June with July not far behind. Furthermore, I conclude that December is the worst time to launch a theater campaign. As for outcomes based on goal amount, I can conclude that campaigns with a goal amount of under $5,000 have a high likelihood of success. The success rate of theater campaigns drops sharply for amounts over $5000. It begins to rise again at $25,000 before dropping off once more at $40,000. It may well be that there is a niche for bigger budget productions.
However, it is unadvisable to make much of this conclusion for reasons given in the limitations section below.

### Limitations
While these two analyses do provide valuable, actionable advice for those looking to use Kickstarter to stage a play, there are limitations to the data -- particularly with the analysis of outcomes based on goals. While the conclusion that the rate of success drops off sharply for campaigns with goals larger than $5000 rests on a solid sample size, not much can be said for theater campaigns with goals larger than $15,000 since the sample size for those campaigns is much smaller. There were fewer than 100 campaigns with a goal above $15000. In fact, there were only 82 campaigns accross the largest seven goal ranges, and only 9 campaigns accross the third and fourth highest categories -- the very categories that seemed to show a sharp rise in the success rate.

As for other limitations, the data from the outcomes based on launch date analysis could be further refined. The data for this analysis consists of all theater Kickstarter campaigns -- not just plays. It may well be that the success rate for opening a theater space at a given time is much different than that of staging a play at a given time. Thus the data may look different if it were limited to plays.

Finally, the data here represented data from all countries. It may have been more useful to the US-based client to filter for US-based campaigns.

### Opportunities Further Analysis

In addition to the two analyses presented, other analyses could be made. One such analysis could determine whether accolades such as being a staff pick or a spotlight production could influence the success rate of a campaign. Possible charts to create would be outcomes based on whether or not a campaign is a staff pick and whether or not a campaign is a spotlight campaign. I might also create boxplots of the analyses I have already done to provide my client with measures of central tendency (mean, median and mode) and measures of spread (standard deviation) as well as outliers.
