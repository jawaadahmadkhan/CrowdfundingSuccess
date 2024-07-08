# Crowdfunding Success on IndieGogo | Data Analyst Project
A data project examining successful crowdfunding campaigns on Indiegogo, utilizing Tableau. (Originally completed July 2023)

## Introduction
In this project, I examine a sample of roughly 20,000 Indiegogo Crowdfunding Campaigns from the years 2011-2020. This dataset was compiled by Kaggle user Quentin McTeer. We examine trends in successful crowdfunding campaigns which can be useful for prospective campaign creators to see what might help bolster success in crowdfunding, particularly utilizing Indiegogo.

## Data Understanding
The dataset includes features of the crowdfunding campaigns including the timeframe they ran for, the category of campaign, the country/geography of the source of the campaign, whether it was fully funded and successful or not, the amount raised, the currency used, and the goal amount each campaign was trying to raise. There is also descriptive data with the URL and text description of the campaigns. After cleaning up unecessary fields and categorization, I've uploaded an Excel workbook with the original dataset, my cleaned version, and Country Data, uploaded as "indiegogo_cleaned_JK.xlsx".

For reference, find the original dataset at Kaggle.com here: https://www.kaggle.com/datasets/quentinmcteer/indiegogo-crowdfunding-data

## Research Problem
In examining this dataset, I explored the question: **What trends are found in successful Indiegogo Campaigns (defined as those that reach their goal)?** This question was examined looking at different features of the campaign (timing, category, and geography). Note that in the findings below, for the regional analysis, I’ve narrowed the data down to the top 4 regions by number of campaigns (those with 900 campaigns or more), as the rest had as little as 1 campaign which wouldn’t be representative for comparison purposes. 

## Findings
In analyzing the dataset, I created a few visualizations to discover trends. See full Tableau workbook, uploaded as CrowdfundingSuccess.twbx and a PDF with a Tableau story as CrowdfundingSuccess.pdf. See findings below:

1. Among the top 4 regions, the United States’ success rate is top, but only by a single percentage point. Canada lags behind at about 4% success, but overall, all campaigns have less than 11% success rate (so it seems region doesn’t show as much of an effect on success rate).

<img width="578" alt="Screen Shot 2024-07-08 at 4 00 29 PM" src="https://github.com/jawaadahmadkhan/CrowdfundingSuccess/assets/63555752/9d1f5e23-c66e-43b3-9b1b-45aafd9994a3">

2.  Looking at categories, we find the most successful categories are a mix of general and specific categories (Audio, Tabletop Games, Camera Gear, Home, etc.). But interestingly, the rate of success didn’t correlate with categories that had more campaigns, rather some categories stood out with a higher success rate given a lower number of campaigns comparatively (specifically Camera Gear and Energy & Green Tech stood out in this regard). On the other hand, there also doesn’t appear to be a correlation between categories with a high number of campaigns and a lower success rate (for example, both Travel & Outdoors and Environment had 806 campaigns, but the former had a 24.6% success rate, the latter only 0.1%).

<img width="537" alt="Screen Shot 2024-07-08 at 4 01 07 PM" src="https://github.com/jawaadahmadkhan/CrowdfundingSuccess/assets/63555752/efb9ae66-17e6-4b84-a5ff-f99291d699f1">

3. Looking at which month of the year campaigns launch and which month they end, June appears to be the top month for both, however the rest of the months don’t match up for success by launch and ending month. There’s not a ton of variation in success rate (only about 3-4% excluding June), but it does appear February has the lowest success rate as a launch month, and September as an ending month (with August being the second worst to launch or end a campaign). 

<img width="492" alt="Screen Shot 2024-07-08 at 4 02 12 PM" src="https://github.com/jawaadahmadkhan/CrowdfundingSuccess/assets/63555752/b04dcc13-d847-47cc-93c3-aa906fcb5c85">

4. Finally, looking at Campaign Length by days, the most success appears to be in campaigns that are 0-9 days long, and 80-89 days long (essentially 3 months). Digging deeper here, I did identify a number of campaigns that raised large amounts of funds in just one day. When digging into those campaigns to find them on Indiegogo, I found that some of them are listed having raised a certain amount, but with the clarification that a large portion had been raised on another platform (e.g. Kickstarter), so these were likely migrated and had the previous funds raised reflected on the campaign. Knowing this, the campaign length data as well as the launch/ending month data may not be as useful (and overall, this led me to look at the data a little more cautiously, as it’s possible further cleanup may be needed to accurately reflect campaigns that specifically raised funds completely on Indiegogo, but overall, we can still glean some useful insights on crowdfunding campaigns overall).

<img width="455" alt="Screen Shot 2024-07-08 at 4 02 36 PM" src="https://github.com/jawaadahmadkhan/CrowdfundingSuccess/assets/63555752/2f804f07-e748-4e80-af29-24cebaa0a848">

## Conclusions & Next Steps

As mentioned above, there are some findings here to examine but there aren't any hugely influential trends among a certain feature like timeframe, geography, or start/end month. However, the data would be interesting for someone to look more into to compare their prospective campaign to it to see the success rates within a certain category of campaigns and if there are any key traits. This can also be taken further by examining campaign data from Kickstarter or LaunchGood for successful crowdfunding campaigns on other platforms.














