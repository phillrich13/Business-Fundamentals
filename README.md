[Tableau dashboard](https://public.tableau.com/views/BoardGameExploration/BoardGameTrends?:language=en-US&:retry=yes&:display_count=n&:origin=viz_share_link), [data](https://docs.google.com/spreadsheets/d/1N-DjsJLlzr47ExjPzLv-RoBvkZrRhgc6mOURbDNmqZw/edit?usp=sharing)
## Proposing a Classification Model for Predicting Successful Board Games

### Abstract
The goal of this project was to create a data science project proposal for a potential real life problem. My focus was on pitching Hasbro to acquire independent board games. The data science solution was to develop a classification model to identify board games with a high sales potential. The target would be a top 20% owned game (using data from the Board Game Geek [BGG] forum as a sales indicator). I explored potential trends in successful board games from the BGG data, and then paired that with industry research.  All of this was done to develop as compelling an argument as possible to implement this classification model as a way to acquire independent board games and increase revenue.

### Design
#### Opportunity
The board games industry is projected to have revenues [exceeding $12 bn by 2023](https://www.prnewswire.com/news-releases/board-games-market---global-outlook-and-forecast-2018-2023-300763553.html), and is projected to have a [compound annual growth rate of ~13% from 2021 - 2026](https://www.reportlinker.com/p05482343/Board-Games-Market-Global-Outlook-and-Forecast.html). This is a rapidly growing market and Hasbro, with a [reported revenue of $5.475 bn](https://www.macrotrends.net/stocks/charts/HAS/hasbro/revenue), has not released many new board games outside of new themed monopoly. [They missed revenue forecasts](https://www.thestreet.com/investing/hasbro-swings-to-first-quarter-profit-misses-on-revenue) in the last quarter, and had a total revenue growth of 0.8%, so now is the perfect chance to delve deeper into the board game market to improve future revenue and meet revenue forecasts. 

#### Solution
Currently there are [over 300 table top games](https://www.kickstarter.com/discover/advanced?state=live&category_id=34&sort=magic&seed=2702421&page=1) looking for funding on Kickstarter. In 2020, the top 10 Kickstarter funded board games and accessories combined to receive over [$55 million in funding](https://www.polygon.com/2020/12/22/22195749/kickstarter-top-10-highest-funded-campaigns-2020-video-games-board-games). In 2019 and 2020 combined, table top games raised over [$400 Million](https://www.polygon.com/2020/12/22/22195749/kickstarter-top-10-highest-funded-campaigns-2020-video-games-board-games) on Kickstarter. By acquiring indie board games Hasbro can capture a larger audience than kickstarter, and through mass production with their pre-existing manufacturing contracts, can increase their revenue.

#### Data Science Solution Path
I believe that by implementing a classification model to identify and prioritize board games with a high probability of success, Hasbro can prioritize games to either invest in or acquire. The target being measured is: Will the game be in the top 20% of sales for that year? By developing a classification model we can capitalize on current patterns in successful board games, and determine more accurate prioritizations for targeting acquisitions.

#### Impact
The classification model will create a prioritization list for acquiring/investing in board games by their sales potential. By acting on this prioritized list, Hasbro can increase their revenue through investing and acquiring board games and providing them to a larger audience.


### Data
I scraped [data](https://docs.google.com/spreadsheets/d/1N-DjsJLlzr47ExjPzLv-RoBvkZrRhgc6mOURbDNmqZw/edit?usp=sharing) from the board game forum, Board Game Geek. I pulled the top 5000 games, and then filtered down to games published from 2010-2020, (~3,200 games). I looked at multiple features including, but not limited to:
* \# of people who own the game
* Year Published
* Game Mechanics
* Game Categories
* Min Age
* Play Time
* \# of Mechanics
* \# of Categories

#### Assumptions

The data comes from the forum, Board Game Geek (BGG). To proxy sales I am using the self-reported ownership counts. This has some caveats in that it doesn't represent total sales, and is limited to people who use the forum (An example is Gloomhaven, which has sold 200k, but has 71k listed owners on BGG)

### Exploratory Methods/Algorithms
Due to the way indie board games are manufactured, the earlier a game was printed, the more opportunities a game has to be re-printed and bought. Because of this, I ranked each game within it's published year based on the number of people who own it. From there I created deciles to account for different amounts of games published each year. I then used these deciles to see how trends have changed over the years, as well as if certain trends were consistent over time. I found a few insightful patterns as seen below:

![Board Game Trends](https://user-images.githubusercontent.com/75561764/119871544-64018780-bed7-11eb-9b17-1142068bb4d1.png)

### Tools
* Python 
  * Beautiful Soup - Scrape HTML to get game IDs
  * BGG API to run through game IDs and get relevant info
* Google Sheets to store, clean, and aggregate data
* Tableau to visualize and organize insights into the data

### Communication
The primary means of communication in this project are through presentation, and a [Tableau dashboard](https://public.tableau.com/views/BoardGameExploration/BoardGameTrends?:language=en-US&:retry=yes&:display_count=n&:origin=viz_share_link)
