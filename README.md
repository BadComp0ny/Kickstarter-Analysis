# An Analysis of Kickstarter Campaigns
Performing analysis on Kickstarter data to uncover trends for successful funding of a new play

## Goals
The primary goals of this exercise is to review prior crowdfunding results to identify if there are commonalities which result in successful crowdfunding campaigns.
Insights found will then be used to plan a new campaign to seek funding for a new play "Fever".

## Analysis 

Initially I reviewed the outcome of all campaigns for plays based on the launch date.
![Image 1](/Theater_Outcomes_vs_Launch.png)
In review you can see that the total number of campaigns for plays begins a steady upward climp in April, reaches an apex in May and comes back down to April levels over the next two months.
As such the optimal time time launch a campaign would is May or Jun.  Based on the data these two months offer over a 65% chance of a successful campaign.
I strongly recommend that we do not consider any campaign start dates after July as the chance of failure increases with each passing month till the end of the year.

The next issue to consider is the funding goals.  The inital budget set for this production was $10,000.  Campaigns with a budget between $5000 & $14999 were only successfuly funded 54-55% of the time.  A significant increase
in success was identified for plays with a goal of $1000 - $4999 and I would recommend a target closer to that amount.
![Image 2](/Outcomes_Vs_Goals.png)

In review of the 1047 campaigns for plays only 158 (15%) had a goal of $10,000 or greater.  Of those 158 only 45% resulted in successfully being funded.

## Challenges Encountered
The data initially presented was rather robust and resulted in some initial challenges to best identify campaigns that were most similar to our objective campaing.
In order to recognize this quickly and easily the data needed to be parsed down to only plays. Additionally all dates in this file were stored in the UNIX timestamp format.
As such the data needed to be formated to be human readable dates.

This data set is also limited in the fact that it simply describes the campaign but does not help identify tactics or perks of the campaign as a crowdfunder.
Did the unsuccessful ones have donation tiers that were too high? Did the successful ones have more opportunities to donate at lower levels?


### Personal Challenges and recommendations

Personally one of the challenges I had with this task was in creating the outcomes based on goals.  Based on prior knowledge I would have used a pivot table and created groups based on the target ranges.
To calculate percentages I would have added another count to show the value as a % of row total.  
![My One Off Work](/Outcomes_Based_on_Goals.png)
The final result isn't as clean as the directed course work and has some risk of 
improperly grouping results but had less risk of improper coding.

Additionally I would recommend reviewing the percentages of success and failure in the theater outcomes based on launch date.  While the 


We only looked at the success based on the goal amount.  As we saw an increase in the number of plays with a goal below our target amount. I would be interested in reviewing pledged amount vs the goal amount.
- How many of the plays with goals less than 10k end up with pledges at or greater than that amount?
- Is there a chance that we could set a smaller goal and still meet our planned budget?
