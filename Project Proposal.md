## Question/need:
*What is the framing question of your analysis, or the purpose of the model/system you plan to build?*


I am looking to work for Hasbro, the toy company, specifically in the boardgames market. My goal is to pitch a potential classification model (top 25% of owned from the data below) for if a game is a good investment or not based on game characteristics. The end goal of this model is to find high sales potential board games to fund.


*Who benefits from exploring this question or building this model/system?*


The boardgames industry is projected to have revenues [exceeding $12 bn by 2023](https://www.prnewswire.com/news-releases/board-games-market---global-outlook-and-forecast-2018-2023-300763553.html), and are projected to have a [compound annual growth rate of ~13% from 2021 - 2026](https://www.reportlinker.com/p05482343/Board-Games-Market-Global-Outlook-and-Forecast.html). This is a rapidly growing market and Hasbro, with a [reported revenue of $5.475 bn](https://www.macrotrends.net/stocks/charts/HAS/hasbro/revenue), has not released many new board games outside of new themed monopoly. [They missed revenue forecasts](https://www.thestreet.com/investing/hasbro-swings-to-first-quarter-profit-misses-on-revenue) in the last quarter, so now is the perfect chance to delve deeper into the board game market to improve future revenue. 

Wizards of the Coast (a Hasbro subsidiary), developer of Dungeons and Dragons, had a [revenue increase of 15%](https://www.thestreet.com/investing/hasbro-swings-to-first-quarter-profit-misses-on-revenue) compared to Hasbro's total revenue growth of 0.8%, showing that even in Hasbro table top gaming revenue is growing steadily. Currently there are [over 250 table top games](https://www.kickstarter.com/discover/advanced?state=live&category_id=34&sort=magic&seed=2702421&page=1) looking for funding on kickstarter. In 2020, the top 10 kickstarter funded board games and accessories combined to receive over [$55 million in funding](https://www.polygon.com/2020/12/22/22195749/kickstarter-top-10-highest-funded-campaigns-2020-video-games-board-games). This means there are plenty of investment opportunities that can help Hasbro reach and exceed future revenue forecasts, and making informed decisions on what games to fund is a key driver for these opportunities. 


## Data Description:
*What dataset(s) do you plan to use, and how will you obtain the data?*

I will use data from Board Games Geek, a user forum for ranking and discussing board games.
Kaggle hosts the data [here](https://www.kaggle.com/mrpantherson/board-game-data)

It contains 4999 rows, 15 columns (~10 useful columns)


*What is an individual sample/unit of analysis in this project?*


An individual sample here is 1 board game


*What characteristics/features do you expect to work with?*


min_players, max_players, avg_time, min_time, max_time, Complexity, avg_rating, geek_rating, num_votes, min_age, mechanic, owned, category, Year


*If modeling, what will you predict as your target?*


The proposed classification model would look to see if a board game could be in the top 25% of BGG ‘owned’ units or not. Basically would it potentially be a top seller based on forum metrics. This is inherently biased but still an indicator of game popularity.



## Tools:
*How do you intend to meet the tools requirement of the project?*


I will host and manipulate the data on google sheets and then more manipulation + visualization in tableau.


## MVP:
A dashboard highlighting trends in genres/other characteristics for games selling well (module project)

A basic classification model (proposed DS project)

