# Capstone 1 - SOCCER & STATSBOMB!

# The Data Source - Statbomb is a business that provides soccer analytics mainly for teams, media, and gambling
https://statsbomb.com

# StatsBomb provides a free dataset to promote furthering soccer and data science, avaiable at https://github.com/statsbomb/open-data

Available data in the free dataset:
* 16 Champions League seasons
* 2 FA Super Cup League seasons
* 2018 World Cup
* 16 La Liga seasons
* 1 NWSL season
* 1 EPL season
* 2019 Women's World Cup

# The Data

Chose to focus on 2018 World Cup
* 64 games - 32 countries
* 48 round robin group stage games - 8 groups of 4
* 16 single elimination games - Round of 16 through Final and 3rd place match

![1- Shape df.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/1%20-%20Shape%20df.png)

![2 - Pass columns.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/2%20-%20Pass%20columns.png)

### **Shout out to this blog for helping me visualize data in some appealing ways:**
https://towardsdatascience.com/advanced-sports-visualization-with-pandas-matplotlib-and-seaborn-9c16df80a81b

# Location, location, location!!

![3 - Pass Map.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/3%20-%20Pass%20Map.png)

![3.1 Pass Map.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/3.1%20Pass%20Map.png)

# Shots too!

![4 - Shot columns.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/4%20-%20Shot%20columns.png)

# France's shots (France was champion)

![5 - Shot Map.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/5%20-%20Shot%20Map.png)

![5.1 shots locations map.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/5.1%20shots%20locations%20map.png)

# Nutmegs? More than you need to know!

![6 - nutmegs.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/6%20-%20nutmegs.png)

# Most important question to answer?

## Messi 2 - Ronaldo 0 - NUTMEGS

![Messi v Ronaldo 4 stats.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/Messi%20v%20Ronaldo%204%20stats.png)

# Focusing on 3 stats! - SHOTS, EXPECTED GOALS, GOALS

![8 - Shots Hist.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/8%20-%20Shots%20Hist.png)

# EXPECTED GOALS STAT
![9.2 - xg tree.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/9.2%20-%20xg%20tree.png)

# Expected goals predicted some very high scoring games and in reality there were some very low scoring games.
![9.0.0.1 xg goals hists.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/9.0.0.1%20xg%20goals%20hists.png)

# This is the story of the tournament - 48 Group Stage games followed by 16 Knockout Stage games
![Actual vs Expected Goals.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/Actual%20vs%20Expected%20Goals.png)

# There seems to be more variation in the Knockout Stage! Let's look at one, the final between France and Croatia

# All of France's shots and the expected goal value
![9 - France xg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/9%20-%20France%20xg.png)

# Here's both teams - The expected goals doesn't tell the tale of actual score
![10.1 France v Croatia xg hists.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/10.1%20France%20v%20Croatia%20xg%20hists.png)

# Expected goals seems questionably correlated to Actual goals
![Expected Goals vs Actual Goals.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/Expected%20Goals%20vs%20Actual%20Goals.png)

# Maybe shots have a better correlation than Statsbomb's Expected Goal? Clearly takes many shots to produce fewer goals
![Goals vs Shots.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/Goals%20vs%20Shots.png)

# Is there a relationship between the tournament average shots/goal and goals per match? There seem to be more disparities than with Expected Goals
![Goals vs Shots Avg](https://github.com/jeromekirkpatrick/capstone_1/blob/main/Goals%20vs%20Shots%20per%20Goal.png)

# Expected Goals investigated further? Do risktakers have higher expected goals?

# Dribblers are risktakers...
![xg vs dribbles.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/xg%20v%20dribbles.png)

# Higher incomplete pass rate is perhaps a sign of risktaking...
![12.1 - pass rate v xg - exploration.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/12.1%20%20-%20pass%20rate%20v%20xg%20-%20exploration.png)

# Nutmegs are definitely a risk, but there aren't enough attempts
![12.2 - nutmegs v xg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/12.2%20-%20nutmegs%20v%20xg.png)


![13 - missed shots.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13%20-%20missed%20shots.png)

![13.1 makes.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.1%20makes.png)

![13.3 - xg averages.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.3%20-%20xg%20averages.png)

![13.4 xg makes > avg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.4%20xg%20makes%20%3E%20avg.png)

![13.4.1 xg makes <= avg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.4.1%20xg%20makes%20%3C%3D%20avg.png)

![13.5 xg misses <= avg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.5%20xg%20misses%20%3C%3D%20avg.png)

![13.5 xg misses > avg.png](https://github.com/jeromekirkpatrick/capstone_1/blob/main/13.5%20xg%20misses%20%3E%20avg.png)






































