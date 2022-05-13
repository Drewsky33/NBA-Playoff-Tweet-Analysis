# NBA-Playoff-Tweet-Analysis

## Project Overview

Every year, the NBA season truly kicks off in the spring time for casual fans. That's no different this year with the NBA playoffs having their best first round ratings in over a decade. A lot of these rating can be attributed to the highly entertaining series between the [Boston Celtics](https://www.nba.com/celtics/) and the [Brooklyn Nets](https://www.nba.com/nets/). This got me thinking about fan's feelings during the course of the playoffs. To answer this question, I set out to scrape tweets from Twitter and visualize the most common keywords from these tweets using word clouds. Since there is a limit of how many tweets I can scrape, I decided to analyze two series, one from the Western Conference and one from the Eastern Conference. I chose the following series for the following reasons:

- Western Conference: [Phoenix Suns](https://www.nba.com/suns/) vs. [Dallas Mavericks](https://www.mavs.com/)
    * I chose this series because the Phoenix Suns are the number 1 seed in the west and are the defending conference champions. I'd like to see how their tweets compare to that of the underdog Dallas Mavericks. 
- Eastern Conference: [Milwaukee Bucks](https://www.nba.com/bucks) vs. [Boston Celtics](https://www.nba.com/celtics/)
    * There's a bit of bias in the series. Personally, I'm a huge Milwaukee Bucks (DEFENDING CHAMPS!). However, they are the underdog in this matchup as the Boston Celtics have had quite the season. The Bucks are the defending champs and have playoff pedigree, but the Celtics have had the better season and are coming of age.
    
## Project Workflow
* Define key functions used to collect and clean data
* I'll have to collect data from Twitter using the Tweepy package in Python. 
* From there I will clean the tweets using NLP (natural language processing)
* List the 50 most frequent words from that data and visualize them with a word cloud
* Identify the optimum number of clusters
* Cluster the tweets using Kmeans and HCA (Hierarchical Clustering Analysis)
* Based on the results of HCA I'll visualize a dendrogram
* Summarize my findings


## Code

The code for this project can be found [here:](https://github.com/Drewsky33/NBA-Playoff-Tweet-Analysis/blob/main/Analyzing%20NBA%20Playoff%20Tweets.ipynb)


## Data

Data was scraped using the `tweepy` package with Twitter API.

## Project Highlights


