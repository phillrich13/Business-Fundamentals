## Proposing a Classification Model for Predicting Successful Board Games

### Abstract


### Design
I am pitching a project to Hasbro to


### Data
I scraped data from the board game forum, Board Game Geek. I pulled the top 5000 games, and then filtered down to games published from 2010-2020, (~3,200 games). I looked at multiple features including, but not limited to:
* \# of people who own the game
* Year Published
* Game Mechanics
* Game Categories
* Min Age
* Play Time
* \# of Mechanics
* \# of Categories

### Exploratory Methods
Due to the way indie board games are manufactured, the earlier a game was printed, the more opportunities a game has to be re-printed and bought. Because of this, I ranked each game within it's published year based on the number of people who own it. From there I created deciles to account for different amounts of games published each year. I then took these deciles to see how trends have changed over the years or if certain trends were consistent over time.


### Tools
* Python 
  * Beautiful Soup - Scrape HTML to get game IDs
  * BGG API to run through game IDs and get relevant info
* Google Sheets to store, clean, and aggregate data
* Tableau to visualize and organize insights into the data

### Communication
The primary means of communication in this project are through presentation, and a [dashboard](https://public.tableau.com/views/BoardGameExploration/BoardGameTrends?:language=en-US&:retry=yes&:display_count=n&:origin=viz_share_link)
