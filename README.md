# An Analysis of Kickstarter Campaigns

## Kickstarter data analysis on theater category, US and GB mainly.

From the 4114 campaigns that we analized, theater had the most kickstarters with 1393.

  -From 1393 theater campaigns 60% were successful Theater is the category with more successful campaigns.

![Parent category](https://user-images.githubusercontent.com/90534703/133912324-4caa3ba1-bfab-4792-badc-6cf348e0bf1d.png)

Focusing on Theater Kickstarters in the US, 525 campaigns were successful of a total of 912.
  -349 campaigns failed.

Now talking about when Louis should launched her project we can said that may is the month with more successful campaigns, followed by June.

![Outcomes based on launch date](https://user-images.githubusercontent.com/90534703/133912320-20acd926-18d1-41bd-b4a6-0431893b8de8.png)

Louis must watch out months like January and October were we can see a bigger number of failed campaigns.


Louise was inspired by five plays she saw at the Edinburgh Festival Fringe and the information that resulted from the analysis is...

  - The successful Kickstarter campaigns have lower goals, almost doubled by the failed campaingns goals.
   
Talking about the musical project in GB, based on our analysis, Louis must produced the play under the budget she is asking for, because half oF the goals are less than $2,000
![GB MUSICAL IQR](https://user-images.githubusercontent.com/90534703/133913889-9c7538a6-42fa-4322-8f2b-78717f47e061.png)


# Kickstarting-with-Excel

Outcomes based on launch dates and goals.

## Overview of Project

### Purpose

Analysis of the relationship between campaings performance and their launch dates and goals.

Get to know the best period of time, in which historically, the campaigns have more success, and also determine the outcomes related with the campaigns goals.

## Analysis and Challenges

This analysis was performed with a data base of different types of campaigns around the world.

![image](https://user-images.githubusercontent.com/90534703/134998422-19720526-a692-413b-9b9d-8167dfc30503.png)

The data base that we have indicates if the campaign was successful, failed, or cancel, but it has more information that help us identify what kind of campaign were those that 
succeed, what characteristics they share. 

In this case Louise only wants to know certain information, how plays behave regarding their launch date and their funding goals.

### Analysis of Outcomes Based on Launch Date

For the Outcomes based on Launch date analysis we did a pivot table. We selected the outcomes, the parent category and the years from our data base.

In this case we only are interested in the theater category, so we just filter the parent category. 

Regarding the years, we are going to focus on the month period, so we had to leave the “month” in the pivot table’s rows.

After we had our pivot table done, we proceed to graphic our information. 


![image](https://user-images.githubusercontent.com/90534703/135000772-e21b69c3-c36b-4be9-ad4a-635291729e08.png)


### Analysis of Outcomes Based on Goals

Regarding the outcomes based on goals, we used the next formula to get the number of campaigns that were successful, failed and canceled.

=COUNTIFS(Kickstarter!F:F,"successful",Kickstarter!R:R,"plays",Kickstarter!D:D,"<1000")

=COUNTIFS(Kickstarter!F:F,"failed",Kickstarter!R:R,"plays",Kickstarter!D:D,"<1000")

=COUNTIFS(Kickstarter!F:F,"canceled",Kickstarter!R:R,"plays",Kickstarter!D:D,"<1000")

Also, as you can see we only considered the “plays” subcategory, because this is the subcategory that Louise is interested in.

And we categorized the funding goals into twelve groups, so we can have a precise result  

![image](https://user-images.githubusercontent.com/90534703/134998500-699ddaa2-fd5a-4087-8752-b39c7db8067b.png)

At the end we transform this information into percentages, so we can see the behavior in a graphic.


### Challenges and Difficulties Encountered

During the analysis I encountered some challenges, the first one was with the Outcomes Based on Goals, after I finished the formulas, I compared the total projects that I 
obtain with the formulas, and the total number of plays projects, and the result was a different number. I had to look for an error, and it was in the last row, in a formula I 
didn’t change the number regarding the goal category.

Another challenge was with the Outcomes by Launch Date, regarding the “month” category in rows, I had to look for information on the internet, and it didn’t take that long, it 
was an easy solution.


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Analyzing the theater campaigns, as we can see in the graphic, May and June are the months in which there was more launched campaigns, also May was the most successful month, 
with a 67% of successful campaigns (111 of 166), followed by June with a 65% of success.

In the other hand we can see that December is a month in which we don’t have an important number of launched campaigns, we just have 75 campaigns, of which 49%, the lowest 
rate, were successful campaigns.

The failed and canceled campaigns are having a standard performance throughout all the months, the failed campaigns moves around 30 and 50 campaigns per month. 

![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/90534703/134109622-4a1401f8-19a3-403a-abb9-d08a946428c2.png)

- What can you conclude about the Outcomes based on Goals?

As we can see in the next graphic the campaigns with lower goals were the ones with a higher success, being those with a goal less than 1000 that got a 76% of success, and the 
ones between 1000 and 4999 with a 73% of success, a total of 388 successful campaigns. These two categories also have the lower rate for failed campaigns.

If we only focus on the graph and the percentage, we can assume that the campaigns with goals between 35000 and 44999 has almost the same successful level, but the total number 
of projects are lower (6 and 3, respectively) compared with the 186 (lower than 1000), and the 534 (1000 and 4999)

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/90534703/134111923-6ee90bac-d420-4c6d-87bb-6a8fa9cca0fa.png)

- What are some limitations of this dataset?

One limitation that this dataset has, is that we can have more information. 

For example, the type of plays, this information can help Louise to have an idea which type of play are more successful, in case she wants a more specific category.

- What are some other possible tables and/or graphs that we could create?

Another table that we can create is one about the outcomes based on the country, so we can see how do the campaigns performed around the world, we could use a histogram.

Other one could be a table with country and pledge, so we can have an idea of where those the campaigns received more pledge.
