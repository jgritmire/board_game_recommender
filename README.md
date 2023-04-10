# Games with Jake (Board Game Recommender)

### Table of contents:

#### Web App :
##### The final product can be accessed at http://flaskexample-env.eba-smpergqp.us-west-2.elasticbeanstalk.com/greet

#### Data:  
##### All data for this project can be downloaded at https://www.kaggle.com/datasets/threnjen/board-games-database-from-boardgamegeek

#### application.py : 
##### This file sets up a flask based web application that functions in the following manner:
##### First, the user input is split into the 3 titles that they input, and is fuzzy matched to our list of possible board games
##### Next, the application retrieves the list of the top 100 recommendations for each game based on both game mechanic similarity, and user review similarity
##### Next, the game mechanic recommendation list and the user review recommendation list are cross referenced to provide the best recommendations
##### Finally, a list of 10 recommendations based on all 3 of the initially input games is returned to the user

#### 1_data_exploration.ipynb : 
##### In this notebook, I explore, visualize, and clean the relevant datasets and prepare them to be used in my product recommender

#### 2_building_product_based_recommer_dataframe.ipynb : 
##### In this notebook, I take the product data and limit it to only the columns that I want to use for my recommender. Then, I calculate the cosine similarity scores between each game based on a variety of variables, and take the top 100 recommendations for each game. This dataframe is then exported as a csv so that it can be quickly accessed in the final recommender. 

#### 2_building_review_based_recommer_dataframe.ipynb : 
##### In this notebook, I take the user review data compiled by Board Game Geek.  Then, I calculate the cosine similarity scores between each user based on a variety of variables, and take the top 100 recommendations for each game based on what similar users rated highly. This dataframe is then exported as a csv so that it can be quickly accessed in the final recommender. 

