# steam-game-recommender-databricks
In this notebook, I build a collaborative filtering recommender system using user data from Steam, a gaming platform. The dataset has four attributes: the user ID, game, user behaviour, and playtime (if the behaviour is play). This data allows us to infer user preferences in the absence of concrete, explicit ratings given by users towards games.

The main goal is to develop a personalised recommender system which uses previous interaction history between user and games to determine which games a user might enjoy in future. The end result should show a list of N games linked to a specific user_id tailored to the user’s unique profile. As the Steam dataset is 200,000 rows, Spark is a good module to use as this can be considered Big Data.

I use the Alternating Least Squares (ALS) algorithm for matrix factorisation, before analysing the performance of the algorithm using metrics such as RMSE and Precision@10. There will also be some examples of hyperparameter tuning, and all of the experiments will be tracked using MLflow.
