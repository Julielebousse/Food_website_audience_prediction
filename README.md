# What features impact the food website audience? 
# Does the meteo impact the audience?
# Can we predict the audience for the next few days?


Description
In this project, I want to understand the features that impact the traffic and the audience of the food website in order to be able to predict the audience in the next few days.

Country : France
Factors chosen : region, Contents_avg_past_2days, evol_content_past_2days, evol_number_users_2days, dayofweek, avg_number_users_2days, avg_ratings, avg_cooking_time, recipe_difficulty, Température, Précipitations, device, cost, bank_holiday, day of week, recipe_media

Workflow
My project can be divided into different phases :

Phase 1 : Looking for a dataset

Research on multiple open data website to find meteo datas

Phase 2 : Cleaning the dataset

My dataset is very large with more than 1 million rows. I need to focus on some features to be more relevant. 
I have categorial data, I need to encode them.

Phase 3 : Visualizing the data

Looking for correlation between our target variable (average rate) and the other variables for a macro analysis --> heat map
Analysis at a more detailed level with different visualizations for each explicative variable

Phase 4 : Analyzing the visualizations & providing insight

Phase 5 : Prediction part

I tried 2 kinds of predictive models Random forrest regressor and XGboost models adding and deleting features to have the best predictions.
I succeeded in having a good prediction using Random forrest regressor adding features such as: averages in the last 2 days (users, pageviews, ratios etc) and the evolution rate in the last 2 days.
To check my model, I looked to MAPE, and I have a result of 16% error.

