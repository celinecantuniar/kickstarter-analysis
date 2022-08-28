# Kickstarting with Excel

## *Overview of Project* 
In this project we created two new analyses: outcomes based on goals and outcomes based on launch date. We created two lime charts: one for theatre outcome based on launch date and one for the percantge for the outcomes of Plays based on their fundraising goal.

### Purpose
We wanted to know how different campaigns fared in relation to their launch dates and their funding goals. Using the Kickstarter dataset that We have already combed through, we visualized campaign outcomes based on their launch dates and their funding goals.

## *Analysis and Challenges*

### Analysis of Outcomes Based on Launch Date
For the first part of the challenge, to visualize outcomes based on lauch date for the Theater catagory, we used pivot tables and a line chart. We created a new column in our main worksheetm for "years" using the YEARS function, then we created a pivot table and filtered it by parent catagory and years. Using the appropriate rows, columns and outcomes and fitering the column labels to only Failed, Successful, and canceled, we created a line chart ot display the data. This line chart was saved as a picture titled "Theater_Outcomes_vs_Launch.png"

### Analysis of Outcomes Based on Goals
For Deliverable 2, the second part of the the challenge we made  seperate worksheet and created our own table. In thi table we used the COUNTIFS function in order to count the number of successful, failed nd cancelled campaigns based on their fundraising goal. We created 12 ranges and then calcualted the total number of projects for ech range using the SUM formula. To get the percentages for each I simply changed the format of the cells to percentage and divided the total  number of campagins by the number of successful, failed and canceled, respectively. 
### Challenges and Difficulties Encountered
I encountered challenges coming up with the COUNTIF formula, and at first did not RE-enter the spreadsheet and column type each time i had to specify the range. For exampe I initially entered this:=COUNTIFS(KICKSTARTER!$D:$D, ">=1000","<=4999",KICKSTARTER!$F:$F,"Successful",KICKSTARTER!$R:$R,"Plays"). Instead of =COUNTIFS(KICKSTARTER!$D:$D, ">=1000",KICKSTARTER!$D:$D,"<=4999",KICKSTARTER!$F:$F,"Successful",KICKSTARTER!$R:$R,"Plays"). I was also unsure wha tthe dollar sign in front of the specified columns meant, so I googled it and essentially all it means is it makes the values An absolute reference; the dollar sign fixes the reference to a given cell, so that it remains unchanged no matter where the formula moves.
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
From my data analysis I can conclude that the most succesfull theatre campaigns were in the month of May, with 111 successful campaigns. Additionally, I can conclude that the number of theatre campaigns overall increaased in the spring months (from March to June) and then see a decline, followed by a short-lived increase in campaigns for the month of October. Overall there were more successful campaigns than failed, throughout the year, and very few canceled.
- What can you conclude about the Outcomes based on Goals?
The main conclusion I can come to based on the Outcomes Based on Goals dataset is that the campaigns with the lower goals tended to be more succesful. As the fundraising goal increased, the percentage of succesful campaigns decreased. However, there is an anomaly in the dataset: when a campaign had a goal of between 35000-40000 dollars, there seemed to be a random increse in successful campaigns, followed by a fast drop in the level of success at the 45000 dollar range. I would consider this to be the "sweet-spot" range for a fundraising goal.
- What are some limitations of this dataset?
One limitation is that we conducted our analysis of only one parent catagory followed by one subcatagory (Theaters and plays). The results might be different for other catagories. The months and time of year can also impact this, for example, plays are likely more successful in the summer because of weather permitting, kids being out of school, and other summer-factors like vacation and time-off work in general. Perhaps a catagory like Radio and Podcasts would see more success during the colder months.
- What are some other possible tables and/or graphs that we could create?
Perhaps a useful dataset to compare catagory vs. time of year/month would be useful. That way we can find out which campaigns are best to run during a specific time of year. This would be best represented in a line graoh with each line representing a catagory, the X-axis being the time of year, and Y-axis being percentage succesful.
