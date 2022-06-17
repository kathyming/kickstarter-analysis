# An Analysis of Kickstarter Campaigns

## Overview of Project
The purpose of the Kickstarter Analysis is to determine two things – is there a better chance of success based on the month a Kickstarter campaign is launched or the goal of the campaign? 

## Analyis and Challenges
### Outcomes Based on Launch Date
* First of all, the goal was to see if there was a better time of year to launch a campaign for a theater project.  Starting with the raw data for Kickstarter campaigns, I created a pivot table which summarized the outcomes (successful, failed, or canceled) for all theater campaigns.  From the data, I created a line graph to depict the outcomes based on month of launch.

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/106352711/174371828-1df9c14a-7689-426a-970b-15258035a0a2.png)

* My biggest challenge was figuring out how to display the Months in the pivot table for Theater Outcomes Based on Launch Date.  At first, I could only list the Year or the Quarter.  I eventually poked around enough to discover I could use the filter for Row Labels.

![Outcomes_by_Launch_Date_Table](https://user-images.githubusercontent.com/106352711/174373154-1fa60c41-f4e8-45b2-baec-2aec11ccb58e.png)

### Outcomes vs Goals
* In order to determine if there is a correlation between goal amount and outcome of campaign, I used the COUNTIFS() function to separate out the campaigns by outcome into categories of goal.  I then determined percentages.

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/106352711/174374123-73c8d883-8ce6-4b04-b914-129744cd8f30.png)

![Outcomes_vs_Goals_Table](https://user-images.githubusercontent.com/106352711/174374921-00e96e1a-e8c2-4009-91a2-f20854a06022.png)

## Results
### Theater Outcomes by Launch Date Results
* June was the most popular month to launch a campaign.
* June also had the highest success rate of all the months.

### Outcomes vs Goals Results
* Success rate declines as goals increase.
* Cancelations slowly rise as goals increase. 

### Dataset Limitations
* The dataset had some extreme outliers.  There were many campaigns with goals of $1.00 which is not a realistic amount in relation to a Kickstarter campaign.  These low goals make the likelihood of success much higher.  There was another campaign with a goal of $100M, which again is an extreme outlier.   
