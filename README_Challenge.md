# Kickstarting with Excel

## Overview of Project
Analyzing and vizualizing campaign outcomes using the Kickstarter dataset. 

### Purpose
To know how different campaigns fared in relation to their launch dates and their funding goals. 

## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/95447175/161151006-6723fa3b-ef54-4688-9488-65ad5251c985.png)

In this first analysis, I looked at the Theater Category outcomes, specifying the number of outcomes – successful, failed, or cancelled based on the Month of the launch. My goal for this analysis was to figure out whether the likelihood of success is related to the Month, and whether some months have a  significantly higher number of successful Theater launches. 

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/95447175/161151014-dd760fef-5885-4d4f-8f8f-680adb236193.png)

In this second analysis, I looked at the percentage of successful, failed and cancelled outcomes based on the Goal amount and the Pledged amount. 
I was looking to find out how the Goal for the play is related to its outcome. I discovered that the Goal amount is in most cases inversely related to the percentage of success. I also did some Descriptive Statistics and found that the standard deviation is higher than the mean, which means that the data are "all over the place", and there is high variability. This is exemplified by the 67% success rates for some plays with higher Goal amounts. 

### Challenges and Difficulties Encountered
I encountered a challenge in modeling the Theater Outcomes by Launch Dates; I was struggling to label the rows in Months and not Years or Quarters. I figured out that I could delete the Quarters while still keeping the Months, and organize the Pivot Table. I figured it out by looking at my previous work for the module, and manipulating the Pivot filters until I got the correct row labels. 
Also, the Countifs() formula was tricky to use, I was getting errors when I first used the formula. I had to use the Hint and follow the link to see how to use the formula. Thankfully, Microsoft explains it very well and it turns out I was stuck on the criteria format – I put >1000 where I was supposed to put ">1000". 

## Results
### Conclusions drawn about the Outcomes based on Launch Date
* May was the best month for successful theater launches, with 111 successful launch dates, the highest number in the analysis
* The number of failed launches and the number of successful launches are very similar in December (37 successful and 35 failed), 
which means that in December there is almost a 50-50 chance of failure or success

### Conclusions about the Outcomes based on Goals?
* It's best to have a Goal of under $20,000; the rate of success goes up as the Goal amount goes down below $20,000
* The rate of success does increase to 67% for Goals of $35,000-$44,999, so other factors may be at play, such as the plot of the play and amount of backers 

### Some limitations of this dataset
* The dataset doesn't show the duration of the proposed projects (plays, musicals, etc.), which may affect their likelihood of succeeding
* The dataset doesn't show how the plays were marketed; nowadays good marketing is very important to sell anything, and if we knew
how the plays in the dataset were marketed, we could make better conclusions about why certain plays succeeded and others failed 
* The dataset doesn't show more granular location data, such as which city each event was in. Some cities are cultural hubs where many people go to see performances, while other cities are in the middle of nowhere and don't get big crowds
* We don't have granular data about the backers, it would be useful to have Target Profiles to know what types of people support each event type, and then use marketing to reach these people and receive more donations

### Possible tables and/or graphs that could be created
* We could compare the donation amount with the amount of backers, to see how they relate
* We could look at event types by country, to see which event type performs best in each country

