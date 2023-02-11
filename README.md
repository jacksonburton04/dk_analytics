# Overview of Repo

Project Completion: Fall of 2020

Outcome: Only tested these lineups on 7-8 DFS games, had around a 50% win rate, but not significant enough of a sample size to draw any conclusions.

# 01_dk_salaries
- The code uses the selenium package to automate the navigation of a website.
- The website navigated is https://www.numberfire.com/nba/daily-fantasy/daily-basketball-projections#_=_
- A Chrome webdriver is used to control the navigation.
- The code clicks on certain elements on the page to reach the desired data.
- The data is scraped and stored as a list of elements.
- The scraped data is converted into a Pandas dataframe.
- The dataframe is cleaned and processed to extract the relevant information.
- The processed data is saved as a CSV file.

# 02_optimize_lineup
- The code is for a DFS (Daily Fantasy Sports) salary optimizer for the NBA.
- It uses the library pulp for linear programming optimization.
- The code starts by loading player data from a CSV file using pandas and cleaning the data by dropping any rows with NaN values.
- Then, the player names are parsed to get the first and last names, as well as the roster position.
- The code then changes the salary column from string to float.
- An array of injured players is created, and these players are filtered out of the data.
- Roster positions are set for the NBA, and a variable is created for each player for each roster position they can play.
- The optimization problem is set up using pulp, with the objective of maximizing projected fantasy points subject to a salary cap constraint and a maximum player constraint.
