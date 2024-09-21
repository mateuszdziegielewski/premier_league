# Analysis of the 2020-2024 Premier League Seasons

#### -- Project Status: Active

## Project Intro
The purpose of this project is to analyze the last 5 seasons of the English Premier League. There are two parts to this project. One focusing on comparing different teams' and formations' performances, including  visualisations and the expected points table for each season. The second part involves a machine learning model predicting match results based on game statistics. Data used in this project can be found [here](https://www.kaggle.com/datasets/mhmdkardosha/premier-league-matches).

### Project organisation:
<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

### Methods Used
* Descriptive Statistics
* Data Visualization
* Machine Learning

### Technologies
* Python

See the [requirements](https://github.com/mateuszdziegielewski/premier_league/blob/main/requirements.txt).

## Project Description

The project is based on the following features from the original dataset:

- *date*: the date of the game
- *round*: the day of the week the game was played
- *result*: the result of the game
- *gf*: goals scored by the home team
- *ga*: goals scored by the away team
- *opponent*: the opponent of the home team
- *xg*: expected goals for the home team
- *xga*: expected goals for the away team
- *poss*: possession percentage of the home team
- *formation*: the formation of the home team
- *sh*: the number of shots by the home team
- *sot*: the number of shots on target by the home team
- *dist*: the average distance of the home team’s shots
- *fk*: free kicks taken by the home team
- *pk*: penalty kicks awarded to the home team
- *pka*: penalty kicks attempted by the home team
- *season*: the season year of the match
- *team*: the home team

In addition, the following measures are derived from them:

- *gdiff*: goal difference
- *xgdiff*: expected goal difference
- *sacc*: shot accuracy
- *shtconv*: shot conversion rate
- *sotconv*: shot on target conversion rate
- *pconv*: penalty conversion rate
- *epr*: efficient possession ratio
- *points*: game result in points
- *exppoints*: expected points calculated from xgdiff
- *last_5*: team's points from the last 5 games

### First Part of the Project:
The first part of the project is an exploratory data analysis combined with the visual comparison of team and formation performance. Created scatterplots show, for example, which teams score more goals, shoot more effectively, or make better use of possession. These insights also allow for an understanding of the possible style and character of particular teams based on the statistics – whether they are more dominant and possession-oriented or more direct, focusing on creating fewer but better goal-scoring opportunities. The same approach has been used to analyze formations, but it's important to note that different teams may play the same formation on paper, making the overall results less precise. Nevertheless, it is still interesting to investigate the potential impact of formations on team performance. The analysis also includes each season's final table, but based on expected points, to show which teams exceeded expectations (performing better than they theoretically should) or underperformed (wasting their chances more frequently). The results clearly show that sport is unpredictable and statistics don’t matter if teams can’t convert them into final results.

### Second Part of the Project:
In addition to the main analysis, the project contains a supervised machine learning model designed to predict the result of each match (win, loss, or draw) based on the provided features. It uses different methods and compares their accuracy:

* Logistic Regression
* Decision Trees
* Random Forests
* K-Nearest Neighbors
* Support Vector Classification (SVC)

### Featured Notebooks:
* [0.01-md-data_cleaning](https://github.com/mateuszdziegielewski/premier_league/blob/main/notebooks/0.01-md-data_cleaning.ipynb) - Dropping unwanted columns, dealing with missing values, identifying and deleting incorrect data records.
* [1.01-md-data_processing](https://github.com/mateuszdziegielewski/premier_league/blob/main/notebooks/1.01-md-data_processing.ipynb) - Adding new columns for future analysis.
* [2.01-md-analysis](https://github.com/mateuszdziegielewski/premier_league/blob/main/notebooks/2.01-md-analysis.ipynb) - The project's core, containing all the visualizations and tables.
* [3.01-md-model](https://github.com/mateuszdziegielewski/premier_league/blob/main/notebooks/3.01-md-model.ipynb) - A supervised machine learning model predicting game results.

### Future Work:
* Simplifying the code: Utilizing more loops and custom functions to improve code readability and reproducibility so it can be used for different projects in the future.
* Further analysis: Extending the current analysis, potentially with hypothesis testing.
* Refining the model: Including more performance metrics, creating a confusion matrix for each method, and identifying the best predictive features.

### License:
The original data, as well as the project itself, are based on the Apache-2.0 license. For more details, check the [LICENSE](https://github.com/mateuszdziegielewski/premier_league/blob/main/LICENSE.txt).
