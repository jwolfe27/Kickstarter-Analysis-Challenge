# Kickstarter Campaign Funding Analysis
---
## Overview
Utilizing a dataset of past kickstarter campaigns, an analysis was performed for Louise containing the Outcome and Success rate of Kickstarter campaigns based on their "Launch Date" and their associated "Goals". The Launch Date analysis was based on the parent category "Theater" which encompasses Plays, Musicals and Spaces while the "Goals" analysis was specific to plays only.

### Purpose
The purpose of this analyis was to provide Louise an understanding of how previous kickstarter campaigns performed based on their launch date and associated funding goal.

## Analysis of Challenges
### Analysis of Challenges Based on Launch Date
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/89044350/131220570-7b92f446-49b6-4a94-bd42-11d95c9188d5.PNG)

Analyzing the data of theaters based on their "Launch Date", we can see displayed in the above line chart that May is the most successful month.  Campaigns launched in September and October show to be the least successful. While there is an increase in failed campaigns for the month of May, it should be noted that a total of 166 individual campaigns were launched during this time period, exceeding any other month.

### Analysis of Challenges Based on Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/89044350/131220586-a7ea84ac-30f5-4b57-9cb6-e355aff6799a.PNG)

Analyzing the data of outcomes based on their "Goals", in the illustration above we can see that campaigns with a goal of $4,999 or less are the most successful, maintaining a success rate of over 70%. It should also be noted that campaigns with funding ranging from $35,000 to $40,000 also experienced a 67% success rate. Campaigns exceeding the goal amount of $45,000 experienced the lowest success rate

### Challenges and Difficulties Encountered
- The initial data received, specific to campaign launch date/end date, required converting the UNIX timestamp to a more readable format.  To do this a column was created to display a more relateable standard date. Looking further, an additional column was created using the =YEAR( ) command to display only the year the campaign was launched.
- Not realizing the need to use ">=" and "<=" while entering the "COUNTIFS" algorithms resulted in inaccurate data retrieval as some campaign goals landed directly on whole dollar amounts, e.g $1000.
## Results
We can conclude from analysis of Outcomes Based on Launch Date that:
- Spring season, more specifically May, is the best time to launch a campaign
- Fall and Winter months, or September through March result in low success rates 

We can conclude from analysis of Outcomes Based on Goals that:
- Campaigns with a goal less than $1000 experience the highest success rate, coming in at 75%.  Note, however, campaigns with a funding goal of $35,000 to $40,000 experienced a 67% success rate, suggesting that other factors, such as Launch Date, come into play.
- Campaigns requiring more than $45,000 showed to be the least successful
## Limitations of this dataset
- The data in this set ranges from 2010 to 2017.  To provide Louise with the most up to date analysis, data from more recent years should be analyzed.
- This analysis could also be more accurate if Louise could provide exactly how long each campaign will be accepting pledges or donations, as each campaign varied in length.
- Lastly, it should be noted that donations are accepted in multiple currencies, requiring currency exchange rates to be taken into account to provide a more accurate depiction of success rate based on Goals.
## Other possible tables and/or graphs:
- A graph focusing on geographical interests comparing the "Blurb" column to the total amount raised or "Pledged". 
