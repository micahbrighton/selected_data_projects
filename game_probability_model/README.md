# Game Probability Model

## TLD;DR
This model predicts the outcome of a simulated basketball game using team stats, opposition stats, and game location.

## Background
I play in online, simulation college basketball league (yes, I know how that sounds). After playing for awhile, I put on my data glasses and started to wonder if there was a way to predict the outcome of a game.

In this specific instance, I wanted the probability of a given outcome instead of the outcome itself since sports are sports and the possibility of an upset is always very real. Using in-universe historical data, I can train and deploy a model to see statistical impacts on the probability of victory.

This model represents my first attempt at building a game probability model for this league. To keep things simple, my first attempt uses a logistic regression model. I know this isn't the most optimal solution, but I wanted to do something fast before the season ended. I will test more advanced machine learning models in the future.

## Inputs
The first model that was built only has 6 inputs:
1. Team Offensive Rating - how many points a team scores per 100 possessions
2. Team RPI - this is representative of how good a team is. It uses team winning percentage, opponent winning percent, and opponents' oppenents winning percentage.
3. Opponent Offensive Rating
4. Opponent RPI
5. Home Court Flag - this indicates whether or not the game is at home. The home team has an advantage of winning.
6. Neutral Court Flag - this indicates whether or not the game was played at a neutral site. Neutral sites do not favor either team.

## Outcomes
