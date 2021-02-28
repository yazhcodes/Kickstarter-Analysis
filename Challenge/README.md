# Kickstarting with Excel

Here's a look at my first Data Analysis project using only the magic of Microsoft Excel, which as it turns out is a much more powerful tool than I ever gave credit for.

## Overview of Project

Over 4000 kickstarter campaigns and their related parameters have been statistically analyzed to uncover hidden crowdfunding trends that ultimately contribute to a campaign's success or failure.

### Purpose

The purpose of this project is to help our client Louise with planning two Kickstarter campaigns. 

1. An American Theatre Play “Fever” with an estimated budget of $10,000. 
2. A British Theatre Musical with an estimated budget of £4,000. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Timing is an important factor when we venture into unclear or risky territories. So the effect the Launching Date will have on our campaign cannot be overlooked. Upon analyzing the outcomes of all Theatre campaigns based on Launch dates and visualizing the results using a Line Chart, it was revealed that the the success rate of campaigns that were launched in the month of May is significantly higher than other months.

<p align="center"><img src="https://github.com/yazhcodes/Kickstarter-Analysis/blob/main/Challenge/Resources/Theater_Outcomes_vs_Launch.png"></img>

### Analysis of Outcomes Based on Goals

The impact of monetary factor to a campaign's outcome is equally important, if not more. So the success, failure and cancelation rates of Theatre plays were analyzed against the Goal of each camnpaign. No Theatre Play campaigns were canceled in the past. So we have only Successful & Failed campaigns to analyze.

<p align="center"><img src="https://github.com/yazhcodes/Kickstarter-Analysis/blob/main/Challenge/Resources/Outcomes_vs_Goals.png"></img>

It's clear from the data that Goals less than $1000 have the highest success rate at 75.8% closely followed by Goals between $1000 and $5000 at 72.6%. One interesting finding is that Goals between $45000 and $50000 have a 100% failure rate. Glad we are not aiming for that figure! Our estimate $10000, has seen a 54% success rate and 46% failure rate, which is inconclusive to determine our campaign's outcome.

But based on the trend lines, it is clear that the higher the goal, the lesser the chance of success and higher the chance of failure.

### Challenges and Difficulties Encountered

The Outcomes by Launch Date chart was a breeze as we had created something similar during the course. When it came to Outcomes by Goals I did face some challenges.

1. I attempted to do this on my own before following the step by step instructions. I ended up with a crowded graph as there were too many Goal values. So I figured I have to find a way to group the goals for better visualization. I researched about binning the goals like we do in Box plots, but couldn't find much. So I came back to the instructions only to see that we had to manually form Groups and use COUNTIFS to finish up!
  
2. Figuring out the COUNTIFS formula was a bit confusing at first but it was easier once I got the hang of it. The fact that I skipped the HINT video did not help. So I had to come back to the video and confirm whether my understanding was correct.

3. Copy pasting the COUNTIFS formula to all the cells and updating the filter conditions to match the context of each cell was a bit frustrating but worth it in the end. I wish there was an easier way to distribute the formula.

4. The Goals vs outcomes chart did not not have significant peaks like Launch Date chart. So I was confused about what I would recommend to my client. But then adding Trend Lines to the chart made a lot of difference to the visualization and made a lot more sense to the data.

5. My biggest challenge so far in this course is figuring my way around Terminal, Github, Gitlab, SSH Keys and what not. I am told this will get easier over time and I sincerely hope so!


## Results

- **Outcomes based on Launch Date:**
	* Our campaign should defenitely be launched in the month of **May** (*or June at the latest*).
	* **December** would be worst time to launch as it has the least success rate. 

- **Outcomes based on Goals:** Trend lines uncover the fact that our campaign stands a better chance with a smaller goal. So I would suggest Louise to cut down as much expense as she can and settle for a lower goal, in order to succeed.

- **Limitations of this dataset:** There are less than 50 US Theatre plays with a Goal between $9000 and $11000. And the outcome is inconclusive with almost equal success and failure rates. If we had had more records in this category, the results might have held more information for us to rely on and decide whether a $10000 goal is a Yay or a Nay.

- **Some other possible tables and/or graphs that I would create:**

	1. The Outcomes vs Goals graph did not make much sense to me until I added the **Trend lines**. This is one addition I would defenitely recommend to understand the data better.
	2. I also added **Data labels** to the peaks in the graph that I discuss about in my analysis report. It's easier for Louise to correlate my findings with the graph when the Data labels are added appropriately.
	3. I would also recommend finding the **difference between Goal and Pledged amount for the failed campaigns** and drill down further into those with bigger gaps. This would reveal the riskiest factors and help Louise eliminate them from her campaign.

