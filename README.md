![Statsbomb](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Screen%20Shot%202020-10-30%20at%204.59.04%20PM.png)

# The Data Source 
# Statsbomb - soccer analytics mainly for teams, media, and gambling
https://statsbomb.com

# Free dataset to promote furthering soccer and data science, avaiable at https://github.com/statsbomb/open-data

Available data in the free dataset:
* 16 Champions League seasons
* 2 FA Super Cup League seasons
* 2018 World Cup
* 16 La Liga seasons
* 1 NWSL season
* 1 EPL season
* 2019 Women's World Cup

# My Dataset

![FIFA World Cup 2018.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/227px-2018_FIFA_World_Cup.png)

Chose to focus on 2018 World Cup
* 64 games - 32 countries
* 48 round robin group stage games - 8 groups of 4
* 16 single elimination games - Round of 16 through Final and 3rd place match


In all, there were over 200,000 rows of events and 121 columns of features being tracked.
![1- Shape df.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/1%20-%20Shape%20df.png)

These are the columns that are tracking pass related features.
![2 - Pass columns.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/2%20-%20Pass%20columns.png)

### **Shout out to this blog for helping me visualize data in some appealing ways:**
https://towardsdatascience.com/advanced-sports-visualization-with-pandas-matplotlib-and-seaborn-9c16df80a81b

# Location, location, location!!
All of a player's passes throughout a game using the player's 'location' and 'pass_end_location'.

![3 - Pass Map.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/3%20-%20Pass%20Map.png)
All of the player's forward passes in the game. Blue are first half and red are second half.
![3.1 Pass Map.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/3.1%20Pass%20Map.png)

# Shots too!
Shots have many associated features being tracked. Including 'shot_statsbomb_xg' which is a stat that Statsbomb came up with to predict how likely a given shot opportunity is to lead to a goal.
![4 - Shot columns.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/4%20-%20Shot%20columns.png)

# France's shots (France was champion)
Using the same method as for passing with the player's 'location' and 'shot_end_location'.
![5 - Shot Map.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/5%20-%20Shot%20Map.png)
Here is a scatterplot of the same shots, which is easier to visualize then the vectors.
![5.1 shots locations map.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/5.1%20shots%20locations%20map.png)

# Nutmegs! More than you need to know?
An extensive number of features being tracked. Top 50 players in the tournament by nutmegs.
![6 - nutmegs.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/6%20-%20nutmegs.png)

# Most important question to answer?
Messi vs Ronaldo!
![Messi v Ronaldo 4 stats.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Messi%20v%20Ronaldo%204%20stats.png)

## Messi 2 - Ronaldo 0 - NUTMEGS




![messi nutmeg.jpg](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/messi%20nutmeg.jpg)



# Decided to focus on 3 stats! - SHOTS, EXPECTED GOALS, GOALS
Somewhat normal distribution. If there were more games, then I'd expect that shots per game would look increasingly normal.
![8 - Shots Hist.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/8%20-%20Shots%20Hist.png)
# All shots across tournament
The penalty spot and penalty kicks explains spike in density
For both misses...
![13 - missed shots.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/13%20-%20missed%20shots.png)
And makes!
![13.1 makes.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/13.1%20makes.png)

# EXPECTED GOALS STAT
This is a breakdown of Statsbomb's factors into rating the 'shot_statsbomb_xg' (expected goal) stat for each shot.
![9.2 - xg tree.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/9.2%20-%20xg%20tree.png)

# Expected goals predicted some very high scoring games and in reality there were some very low scoring games.
![9.0.0.1 xg goals hists.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/9.0.0.1%20xg%20goals%20hists.png)

# This is the story of the tournament - 48 Group Stage games followed by 16 Knockout Stage games
There seems to be more variation between goals and expected goals in the Knockout Stage. I wonder why!
![Actual vs Expected Goals.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Actual%20vs%20Expected%20Goals.png)

# Looking further at expected goals in one Knockout Stage game - The Final between France and Croatia

# All of Croatia's shots and their expected goal value
As you can see, Croatia had 15 shots, and almost all of them, except one, had low expected goals values. The one relatively high value, .55, was when France's goalkeeper made a mistake for a pretty easy opportunity for Croatia.
![Croatia_xg2.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Croatia_xg2.png)

# Here's both teams - The expected goals (1.06-1.25) doesn't tell the tale of actual score (4-2)
![10.1 France v Croatia xg hists.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/10.1%20France%20v%20Croatia%20xg%20hists.png)

# Expected goals seems somewhat correlated to Actual goals, would hope very correlated...
They seem to have some correlation in this scatterplot.
![Expected Goals vs Actual Goals.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Expected%20Goals%20vs%20Actual%20Goals.png)

# However, do shots have a better correlation than Statsbomb's Expected Goal?
Here you can see that it takes many shots to produce a goal. Actually a 10.1 shots/goal average in this tournament.
![Goals vs Shots.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Goals%20vs%20Shots.png)

# Then, is perhaps average shots/goal a better predictor of goals per match? 
Looks like there is discrepancy between average shots/goal and actual goals.
![Goals vs Shots Avg](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Goals%20vs%20Shots%20per%20Goal.png)

# Expected Goals investigated further! Do risktakers have higher expected goals? REDHERRINGS AHEAD.

# Dribblers are risktakers...
![xg vs dribbles.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/xg%20v%20dribbles.png)

# Higher incomplete pass rate is perhaps a sign of risktaking...
![12.1 - pass rate v xg - exploration.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/12.1%20%20-%20pass%20rate%20v%20xg%20-%20exploration.png)

# Nutmegs are definitely a risk, but there aren't enough attempts
![12.2 - nutmegs v xg.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/12.2%20-%20nutmegs%20v%20xg.png)

# Re-focusing on just goals, shots, and expected goals

# Let's do a linear regression to see how great Expected Goals are at predicting Actual Goals:

![Expected Goals vs Actual Goals with fit line.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Screen%20Shot%202020-10-30%20at%204.44.38%20PM.png)

# The numbers of the linear regression calculations
![Linear Regression expected goals vs actual goals.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Linear%20Regression%20expected%20goals%20vs%20actual%20goals.png)

# Expected Goals vs Shots is interesting to consider too
![Expected Goals vs Shots w/fit line.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Expected%20Goals%20vs%20Shots%20w:fit%20line.png)

# Those numbers
![Linear Regression expected goals vs shots.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Linear%20Regression%20expected%20goals%20vs%20shots.png)

# The residuals look strange!
![Residuals.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Residuals.png)

# Does the QQ Plot suggest some non-linearity?
![QQPlot.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/QQPlot.png)

# If non-linearity, could strangeness between Expected Goals and Actual Goals during the Knockout Stage as the bar chart suggested

![Actual vs Expected Goals.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/Actual%20vs%20Expected%20Goals.png)

# Let me get see how Expected Goals vs Actual in the Group Stage only looks...

# Wait this is proving hard... I'm not getting the goals I expect between the Group Stage and Knockout Stage...

# Google, how many goals were there in Knockout Stage? Google, this shouldn't be so hard!

# Wait?! What? There were 169 total goals in the whole tournament, 

![FIFA goals = 169.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/FIFA%20goals%20%3D%20169.png)

# not 183 as my dataset says...

![all_df goals = 183.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/all_df%20goals%20%3D%20183.png)

# Maybe these are shots that went in the goal, and were called back due to an infraction...
There is no offside stat that I can find, and that is a frequent reason goals get called back. So I don't think goals are being called back.

Maybe I made a mistake in joining the dataframes? I don't think so though. None of the games were repeated in the data as far as I can see.

# The top scorer had 6 goals, not 7??

![FIFA top goal scorer = 6.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/FIFA%20top%20goal%20scorer%20%3D%206.png)

![all_df top scorer = 7.png](https://github.com/jeromekirkpatrick/Goals-Expected-Goals-and-Shots-of-2018-World-Cup/blob/main/images/all_df%20top%20scorer%20%3D%207.png)

# Learning this all at 2pm shortly before presenting... Well, something is going on and it's either me or this dataset!
This will take further exploration to figure out why the dataset seems to have more goals than the actual tournament before I dig further into expected goals during the Knockout Stage.

# Biggest Takeaways:
# * Get the assumptions wrong and all the conclusions are spoiled
# * Expected a stat like 'goal' to be unambiguous, and that proved an assumption I almost didn't question in time

# Wishes:
# * Offside calls
# * VAR (Video Assistant Referee) data. One of the big stories of 2018 World Cup.
# * 'Goal' being it's own column.

# Thank You's!
Thanks to Jamie for walking me through linear regression! Thanks to Hashim for being soccer datasets buddies and being there to bounce ideas off! Thanks to my group for being chill to work beside! Thanks to my family for hugely supporting me while I concentrate as much as possible on this class and project!




























































