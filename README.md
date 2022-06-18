Refactor VBA code and measure performance

Purpose of Analysis

The purpose of this analysis was to refractor the VBA code origianlly created to analyze the performance of the list of stocks for 2017 and 2018, and to determine of the refractored code improves the performance and runs the analysis faster.

![LinkedImage](.\resources\green_stocks_2017.png)
![LinkedImage](.\resources\VBA_challenge_2017.png)
![LinkedImage](.\resources\green_stocks_2018.png)
![LinkedImage](.\resources\VBA_challenge_2018.png)
![LinkedImage](.\resources\All_Stocks_2017.png)
![LinkedImage](.\resources\All_Stocks_2018.png)

How to Perform the Analysis

To perform the analysis of theater outcomes relative to launch dates, I made a pivot table of the data, with Outcomes in the columns
section and the Date Created listed by month in the row section. The data was filtered by the parent category of Theater. Theater 
outcomes, either Successful, Failed, or Canceled, were plotted by month is a line graph.

To perform the analysis of fundraising outcomes relative to fundraising goals, I used the COUNTIFS function to enumerate the number of 
successful, failed, and canceled outcomes relative to goals, delineated by dollar ranges.

Challenges and Difficulties

This work involved potential challenges and difficulties. One of the challenges was to convert the launched_at date to a standard 
readable date. The launched_at date was in the form of the Unix or Epoch time, or the number of seconds elapsed since 00:00:00 UTC 
on Jan. 1, 1970. A formula had to be devised and implemeted in Excel to convert each of these Epoch times to a readable date in 
the format of day, month, and year.

Another challenge to overcome was figuring out the correct format of the pivot tables. As pivot tables could be designed in an 
infinite variety of ways, organizing the data to get meaningful results could be challenging to people with limited experiences with
pivot tables. As one gains more experience with pivot tables, pivot table design becames easier and more natural.

Conclusions

One can draw several conclusions bout Theater Outcomes by Launch Date. First, successful theater campaigns are more likely to occur 
during spring and summer months than during fall or winter months. This is because the line graph of successful outcomes (in blue) 
rises sharply through the spring months of March and April and peaks in May, then begins a steady decline through the summer 
until September. After a short rise in October, the rate of successful campaigns drops sharply through the remainder of the year,
reaching its lowest point in December.

Second, failed and canceled theater campaigns show less seasonal variation than successful campaigns. The graphs of failed outcomes
(in red) and canceled (in yellow) show less prominent peaks and little discernable seasonal variations.  

The general conclusion is that when the goals are relatively low and modest in number, the goals are more likely to be successful.
However, as the goal numbers increase in value, then they become more challenging to achieve, so success rates are lower. 

Data Limitations and Possible Future Work

The data is limited by the relatively small number of values, particularly at high numbers. There are less than 100 campaigns overall 
with goal values of $15,000 or higher. It may be a good idea to assess why a high percentage of the campaigns fail. The most likley
reason is that the goal values appear to be set too high, so a feasible solution may be to reduce these goal values to lower and
more realistic values that would achieve a great chance of success.

One could analyze the data further by creating additional graphs using different columns of data. In our analysis, we examined theater
outcomes based on launch dates, with the graphical pattern showing that theater outcomes have the most successful outcomes when 
launched during spring and summer months. 

In a different analysis, we could apply the data column backers_count to see if the number of backers has a positive influence on
whether or not campaigns are likely to succeed. A quick, cursory check of the data using pivot table analysis indicates that 
campaigns with more backers more likely to succeed, as one would expect. To plot this data more clearly and concisely, one would 
group the number of backers into ranges (i.e. <5, 5-10, 11-20, etc.) and make pivot tables and charts.

