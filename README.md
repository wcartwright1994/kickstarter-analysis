# kickstarter-analysis
Performing analysis on Kickstarter data to uncover trends

**Overview of the Project**

The purpose of this analysis is to determine the outcomes of fundraising goals for different Kickstarter campaigns based on their launch dates and fundraising goals. Based on information provided, the focus will be on cmapaigns dealing with the theater, more specifically plays.

**Analysis and Challenges**

_Analysis Description_
  1. Based on the available data, it appears that campaigns launched during the summer have a higher success rate than campaigns launched during other times of the year. In addition, more campaigns appear to be launched during this time. The lowest success percentage is in December with 49% and the highest success percentage is in may with 67%. The average success percentage across all months is 61% with a standard deviation of 4.4%. Based on the available data, Louise would have the higher success rate by holding her fundraising campaign during the summer.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/82549092/115318861-a0a9c880-a14c-11eb-8fdc-7d9ae52f0f7a.png)
  
  2. There exists a negative correlation between success rate and fundraising goal based on the available data. None of the fundraising campaigns for the "Theater: plays" category have been cancelled based on the available data. Based on the available data, Louise would have the higher success rate with a lower fundraising goal.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/82549092/115318855-9ee00500-a14c-11eb-9d6a-f3759fbd690a.png)

_
Challenges or Difficulties_
 1. Creating the countifs formulas for "Outcomes Based on Goals" was tedious and would requires multiple formula updates if the ranges were changed. To aleviate this, min and max range columns were created for the formula to reference for ease of calculation and update.
 2. Althought the goal and pledged columns are formated with a "$" sign, there is also a column for the currency of the campaign. The dataset does not provide details on if the goal and pledged monetary values are actually converted to the same currency, although the columns are formatted to appear as USD. This could result in misinterpreations of the bucketing for the "Outcomes Based on Goals" analysis.

**Results**

_Theater Outcomes by Launch Date_
  1. The largest amount of campaigns, as well as the largest percentage of successful campaigns, were created in May.
  2. Compared to succesful or failed campaigns, very little theater campaigns were cancelled.

_Outcomes based on Goals_
  1. "Theater: plays" campaigns with a goal under $19,999 has a success rate of over 50% based on the available data.
_
Summary of Limitations on Dataset_
  1. **Theater Outcomes by Launch Date** - Louise's analysis should be performed on the percentage of successful projects compared to only number of projects. Although the month with the most successful projects also aligns with the highest percent of success in the current dataset, this could be different in other years. In addition, layering in the additional category of fundraising goals could paint a different picture based on how much campaigns were looking to raise during particular months.
  2. **Outcomes Based on Goals** - Across the sample data, most of the data is concentrated on campaigns with a goal of less than $10,000. Without knowing Louise's goal, we are unable to know if our analysis will be relevant. If Louise had a goal that was greater than $25,000, there may not be enough data to perform accurate analysis. 

_Recommendations for additional tables or graphs_
 1. Adding a table with currency exchange rates per day over the dataset period, as well as labeling the goal and pledged column header with either local or USD, would allow for Louise to more appropriately determine if the data was already converted to USD for analysis.
 2. Adding a line graph showing average donation over time would be helpful for Louise to determine if there is strong ongoing support for "theater: plays" campaigns. This would be helpful if Louise is considering participating in future campaigns.
