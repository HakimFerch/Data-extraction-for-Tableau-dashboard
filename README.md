# Data-extraction-for-Tableau-dashboard
Extracting,Cleaning and transforming data pulled from football-data.org RestfulAPI to use later in building a Tableau dashboard. 
## Tableau public dashboard link: https://public.tableau.com/profile/hakim.ferchichi#!/vizhome/ChampionsleagueDashboardfootball-data_orgAPI/Dashboard1

My deep passion for both football and data drove me to think of a project that brings both sides together and consequently provide an answer to a question of mine which is: 

**"Which clubs were the most performing during the last 3 seasons in the UEFA Champions League?"**.

## Skills used:
* ETL (Extract,Trasnform,Load)
* Data Visualization
* Dashboard design

## Technologies:
* Python (Jupyter notebook)
* Tableau Desktop
* Excel

I used the football-data.org v2 API, a public free to use API which contains data of over 147  official football competitions worldwide starting from the 2018/2019 season.This project however encapsules only the UEFA champions league competition the most competitive and prestigious championship in the footballing world.


I followed The football-data.org's official website contains documentations (https://www.football-data.org/documentation/quickstart) on how to navigate the API and extract specific data using python through API requests.

I used python to pull the champions league data using the requests library, then collect different resouces through filters listed in the documentation. My aim was to build dataframes about all the matches played and the highest scoring players during the last 3 seasons to later use in as data source for the Tableau dashboard.

The data provided by the API ususaly comes in JSON format, so i had implement functions to extract details relevant to the project, clean and organize data, then transform it depending on the use case.

The final output is a data source to load into tableau which contains 3 CSV files:
* 'top_scorer.csv'  providing details about the highest scoring players.
* 'stats.csv' listing every team's stats ('Winning percentage','Goals for','Goals against','Matches played')
* 'CL matches.csv' contains all details of the 604 matches played over the last 3 seasons.

The dashboard consists of 4 barcharts of the 4 metrics i chose to assess teams performance :

* Matches played
* Winning percentage
* Goals scored per match
* Goals against per match
 
 It also contains a Table of the highest scoring players details (Name, Nationality, Position, Teams, Number of goals).









