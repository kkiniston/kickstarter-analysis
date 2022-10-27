# kickstarter-analysis
Preforming analysis on Kickstarter data to uncover trends 
# Kickstarting with Excel

## Overview of Project

### Purpose
  The purpose of this analysis was to help Louise's project campaign and better vizualize the dataset provided in a more understandable fashion. Working with larger datasets can create an array of difficulties in understanding what the data is saying. Using Excel we are able simply organize and vizualize the data for Louise so she can easily see campaign outcomes compared to how well they succeeded and use those trends to build a stonger timeframe to goal ratio for future play campaigns. 
  Throughout this analyis multiple codes and vizual aids are used to breakdown the data so we can better compare how other campaigns faired in the alloted timeframe. Using:
  ```
  PivotTables, 
  ```
  ```
  COUNTIFS()
  ```
  ```
  SUM()
  ```
  Functions, We are able to organize the data set on a line graph the data displayed showing the outcome of theater campaigns compared to their launch date and trends based on what outcomes resulted from a reported goal. 
  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
  First organizing the Kickstarter data set utalizing a PivotTable we are able to manupulate the specific data that we want to display. In this case for Louise we want to first filter the data set based on the Parent Category type *Theater* and our year. Focusing on the count of outcomes we can orgaize the table to show how well they compared in a month by month display. 
  
  ![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/115853964/198193578-859e8d75-fc16-4b7a-bd7a-2c59a6823f9c.png)
  From this data we can see that the peak of successful campaigns were in the months of **May** and **June**. This trend is similarly followed in the grand total of campaigns showing us the more ideal time frame to run a more succesful campaign would be in the end of spring and early summer. This trend can be backed by an eagerness in the community to get out following colder weather which is why we see a similar trend in the fewer number of overall campaigns in the colder months. 
  

### Analysis of Outcomes Based on Goals
  Organizing the data set using code such as:
  
```
=COUNTIFS(Kickstarter!D:D, ">=1000",Kickstarter!D:D, "<=4999", Kickstarter!F:F, "successful", Kickstarter!Q:Q, "plays")
```
 The data set is able to be organized based in percentage based outcome showing how well campaigns did compared to a specific goal range. The data set is further organized to display the number of *successful*, *failed*, and *canceled* plays and the number of plays in a specific goal block.
 
 ![Outcomes_vs_Goals](https://user-images.githubusercontent.com/115853964/198195216-d41dcdde-299e-423d-8fbe-a277fb4dca09.png)

  Using this data we can see that by pulling from our original data worksheet the numper of applicable projects for Louise's campaigns are displayed in a line graph. The number of successful campaigns favored a campaign goal of $10,000 or less. On the other hang there was a larger number of campaigns with the largest campaign goal of $50,000 or more that failed. There were no canceled play campaigns.

### Challenges and Difficulties Encountered
  The largest challenge I faced was small technical errors, usally in my filtering of specific columns that would drastically change my results. Working with larger sets of data and complex functions utilizing other sheets one thing off and my information was completely wrong. This happened when I was creating the **Outcomes Based on Goals**, my data was flipped and showing a more elongated graph. I knew this wasn't right so I back tracked and checked all my functions and found the error in one of my conditions. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
   The first conclution I can make about the **Outcomes based on Launch Date** is that Louise would have the best luck with a campaign in May or June, the begining of nicer wether when people are more likely to be out. The second conclution following a similar trend is the velocity during the holidays drastically decreases including an increase in the number of cancled campaigns. 

- What can you conclude about the Outcomes based on Goals?
   Based on the **Outcomes based on Goals** I can conclude that most succcessful goal range was $25,000 to $30,000. There were more successful campaigns with a lower and more reasonable campaign goal while a larger number of failed campaigns hosted a larger goal. Although the data fluctuates regularly based on goals there are no canceled camapaigns. 

- What are some limitations of this dataset?
        This dataset may be limited in the how further the Subcategories can be broken down. Looking at the **Outcomes Based on Launch Date** we see a very human trend being followed. We can further break this down by type of play and may have completely different results for the ammount of successful plays during the colder months if they are predominatly holiday based plays. 
- What are some other possible tables and/or graphs that we could create?
     We can also use a Stacked Bar graph to easily display the ammount of *Successful*, *Failed* and *Canceled* campaigns in a Month by Month format. 
