# Acquisition Model Proposal

## Opportunity
The board games industry is projected to have revenues [exceeding $12 bn by 2023](https://www.prnewswire.com/news-releases/board-games-market---global-outlook-and-forecast-2018-2023-300763553.html), and is projected to have a [compound annual growth rate of ~13% from 2021 - 2026](https://www.reportlinker.com/p05482343/Board-Games-Market-Global-Outlook-and-Forecast.html). This is a rapidly growing market and Hasbro, with a [reported revenue of $5.475 bn](https://www.macrotrends.net/stocks/charts/HAS/hasbro/revenue), has not released many new board games outside of new themed monopoly. [They missed revenue forecasts](https://www.thestreet.com/investing/hasbro-swings-to-first-quarter-profit-misses-on-revenue) in the last quarter, and had a total revenue growth of 0.8%, so now is the perfect chance to delve deeper into the board game market to improve future revenue and meet revenue forecasts. 

## Solution
Currently there are [over 300 table top games](https://www.kickstarter.com/discover/advanced?state=live&category_id=34&sort=magic&seed=2702421&page=1) looking for funding on Kickstarter. In 2020, the top 10 Kickstarter funded board games and accessories combined to receive over [$55 million in funding](https://www.polygon.com/2020/12/22/22195749/kickstarter-top-10-highest-funded-campaigns-2020-video-games-board-games). In 2019 and 2020 combined, table top games raised over [$400 Million](https://www.polygon.com/2020/12/22/22195749/kickstarter-top-10-highest-funded-campaigns-2020-video-games-board-games) on Kickstarter. By investing in and acquiring indie board games Hasbro can capture a larger audience than kickstarter, and through mass production with their pre-existing manufacturing contracts, can increase their revenue.

## Solution Path
### Data Science Solution
I believe that by implementing a classification model to identify and prioritize board games with a high probability of success, Hasbro can prioritize games to either invest in or acquire. [Through exploratory analysis](https://public.tableau.com/views/BoardGameExploration/BoardGameTrends?:language=en&:display_count=y&publish=yes&:origin=viz_share_link) of data from the leading boardgame forum (Board Game Geek), a few clear patterns have emerged. For example, the more categories a game falls into the more people buy it. Also, identifying the top categories can inform which categories are prized the most in acquiring or investing. By developing a classification model, we can capitalize on these patterns and come up with more accurate prioritizations for targeting acquisitions and investing.

![Screen Shot 2021-05-25 at 1 15 38 PM](https://user-images.githubusercontent.com/75561764/119562560-51624380-bd5b-11eb-9907-4638d2623312.png)

### Impact
The classification model will create a prioritization list for acquiring/investing in board games by their sales potential. By acting on this prioritized list, Hasbro can increase their revenue through investing and acquiring board games and providing them to a larger audience.

### Risks
With the classification model, Hasbro will be investing in a board game before knowing public interest. Kickstarter, by its crowd-funded nature, forces there to be interest in the product to actually be published. So while Hasbro has a wider audience reach than kickstarter, it has to invest in manufacturing and publishing based solely on the model and potentially qualitative review. The model should reduce some of this risk, but it is still inherently more risky than the kickstarter method. There is also the risk of alienating board game enthusiasts who prefer the current small scale of indie board game distribution.

### Assumptions
The data comes from the forum, Board Game Geek (BGG). To proxy sales I am using the self-reported ownership counts. This has some caveats in that it doesn't represent total sales, and is limited to people who use the forum (An example is Gloomhaven, which has sold 200k, but has 71k listed owners on BGG) 
