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

## Research Questions:

# Research Questions
- Which players have fans been tweeting about the most?
- Which team seems to have the advantage?
- Have there been any key events in each series?
- What words seem to be trending the most in each series?


## Code

The code for this project can be found [here:](https://github.com/Drewsky33/NBA-Playoff-Tweet-Analysis/blob/main/Analyzing%20NBA%20Playoff%20Tweets.ipynb)


## Data

Data was scraped using the `tweepy` package with Twitter API.

## Project Highlights

### Scraping Tweets

<img width="651" alt="image" src="https://user-images.githubusercontent.com/77873198/168199792-971f94e1-5cb2-4dd3-82c9-9a188f67d61e.png">

### Cleaning and Visualizing Tweets with a Wordcloud

<img width="575" alt="image" src="https://user-images.githubusercontent.com/77873198/168199958-ac1bb711-96bb-4b9d-8bdb-c69c763daed5.png">

### Clustering Tweets

#### Determining Optimum Clusters

<img width="503" alt="image" src="https://user-images.githubusercontent.com/77873198/168200126-3b4a955b-0284-4a9f-9746-26bf942f8c51.png">

#### Clusters

<img width="509" alt="image" src="https://user-images.githubusercontent.com/77873198/168200231-2d08e39b-1a07-4851-b70e-5f4118ff23a1.png">

### Creating Dendrograms

<img width="945" alt="image" src="https://user-images.githubusercontent.com/77873198/168200378-9bc84f9c-396d-4ff6-bfd8-16b75eb90e5a.png">


## Conclusions

In this project I wanted to scrape tweets related to two series currently happening in the NBA right. I used those tweets to create word clouds of the 50 most popular words related to each team hashtag. After that, I tried to cluster the tweets into groups based on their similarities. This was accomplished through K-means clustering and HCA. Here were my findings from each step of my analysis:

- Word Clouds:
    * Bucks fans tweeted about Giannis Antetokounmpo their best player and Al Horford the opposing teams best player who played exceptionally well in the series so far. 
    * Celtics fans also tweeted about Al Horford, but also tweeted about the refs and the big comeback in Game 5 by the Bucks.
    * Suns fans tweeted about ticket giveaways, retweeting, and Chris Paul
    * Mavs fans tweeted about NFT collections, betting, and but I suspect the hashtag used to scrape in Tweets wasn't a good hashtag. 
- Clustering:
    * The clusters generated for the Eastern Conference had pretty clear clusters and the words within most of the clusters seemed to be related. The best cluster was the final one which talked about the broadcast of the game. 
    * The clusters generated for the Western conference were not very strong in their accuracy. This could be because of the excessive amount of people tweeting about giveaways or NFT's, or sports betting. 

- Addressing Research Questions:
 * Which players have fans been tweeting about the most? **Giannis Antetokounmpo was the player who seemed to have the most tweets about him.**
 * Which team seems to have the advantage? **The Bucks had the advantage based on tweets from both Milwaukee and Boston fans. The other series, it wasn't clear because the cluster weren't clear.** 
 * Have there been any key events in each series? **Boston fans tweeted about the refs and a comeback.**
 * What words seem to be trending the most in each series? **For MilvBos it was Horford** and for **PHXvDal** it giveaways or NFT collections
 
## Next steps:
- This project was interesting. Some next steps for project ideas could be:
    * sentiment analysis
    * visualizing kmeans clusters



