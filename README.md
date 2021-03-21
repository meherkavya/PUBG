# PUBG

**PUBG - Player Unknown’s Battleground (FINISH PLACEMENT PREDECTION).**
**Introduction**
Player Unknown Battle Ground’s (PUBG) is an online Multiplayer battle royale game developed by
PUBG Corporation. It is a player versus player action game in which no more than 100 player fight in a
battle royale. Players can choose to enter the match solo, duo or with a small team up to 4 people. We
will address this discrepancy during feature engineering. The last person or the last team alive wins the
match.

The data is part of a Kaggle competition which has scraped 65000 games worth of data using an API. The
goal is to predict the win percentage of the player based on 28 given features. For example, in a solo
game of 100 players if a player got rank of 80, then its winPlacePerc will be (100-80)/(100-1)=0.204
using the formula winPlacePerc = (maxPlace-winPlace)/(maxPlace-1). The problem is then essentially a
regression problem to predict the winPlacePerc of the player between [0,1].

These types of problems are solved by doing extensive exploratory data analysis and feature engineering
before applying a regression model. We were provided with the Training Dataset so we divided it into
Training and Validation Dataset in 70:30 ratio respectively. We first used the LGBM (Light Gradient
Boosting Machine) (5) Regressor to train our training dataset after doing exploratory analysis on the data.
We compared other models with the same dataset. We reported the accuracy of each model that we got
on the validation data.

**Pre-requisite**
Hands-on knowledge of Numpy, Scikit learn, Matplottlib, Seaborn and Pandas is essential
before working on the Project.

**Objective**
To predict the final ranking and placement from the game statistics and the initial player ratings.
The overview of the steps involved in the project is:
- Data Cleaning and Exploratory Data Analysis
- Visualizing the data and feature engineering
- Training Models on Training data and then drawing comparison between them using validation data
- Choosing the best model and fitting the Test data on it
- Reporting the Accuracy of the final chosen model.

**Data Set**
Training set – 4.45 million
Test Set – 1.93 million
Features – 28
Target -1
