# Title: Retail Sales Prediction
#Introduction:The word sales refers to exchanging goods and services, also known as commodities, for money. More specifically, the definition of retail sales is the selling of desirable goods, usually in small quantities, to the general public for their own personal consumption.
# Problem Statement:
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied. My work includes various plots and graphs , visualizations , feature engineering , ensemble techniques , different ML algorithms with their respective parameter tuning , analysis and trends . Predictions are of 6 weeks of daily sales for 1,115 stores located across Germany.

In this project, the Kaggle Rossman challenge is being taken on. The goal is to predict the Sales of a given store on a given day. Model performance is evaluated on the root mean absolute percentage error (MAPE).

The dataset consists of two csv files: store.csv and train.csv

Data Files:

train.csv holds info about each store. store.csv holds the sales info per day for each store.

The repo contains main.py that runs the main script from step one until the end.
# Bussiness Problem:
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.
# Solution Strategy:
My strategy to solve this challenge was:

Step 01: Data Description: Use statistics metrics to identify data distributions.

Step 02: Feature Engineering: Derive new attributes based on the original variables to better describe the phenomenon that will be modeled.

Step 03: Exploratory Data Analysis: Explore the data to find insights and better understand the impact of variables on model learning.

Step 04: Feature Selection: Selection of the most significant attributes for training the model.

Step 05: Machine Learning Modelling: Machine Learning model training.

Step 06: Hyperparameter Fine Tunning: hoose the best values for each of the parameters of the model selected from the previous step.

Step 07: Convert Model Performance to Business Values: Convert the performance of the Machine Learning model into a business result.
# Machine learning Models:
Lasso& Redige Regression
Decision Tree
Random Forest Classifier
# We predict that Random model is best model for this data.
# conclusion:
CONCLUSION   FROM  EDA

1) From plot sales and competition Open Since Month shows sales go increasing from November and highest in month December.
2) From plot Sales and day of week, Sales highest on Monday and start declining from Tuesday to Saturday and on Sunday Sales almost near to Zero.
3) Plot between Promotion and Sales shows that promotion helps in increasing Sales.
4) Type of Store plays an important role in opening pattern of stores.
5) All Type ‘b’ stores never closed except for refurbishment or other reason.
6) All Type ‘b’ stores have comparatively higher sales and it mostly constant with peaks appears on weekends..
7) We can observe that most of the stores remain closed during State Holidays. But it is interesting to note that the number of stores opened during School Holidays were more than that were opened during State Holidays.

Conclusion From model 
We saw that Sales column contains 172817 rows with 0 sale. So we created a new data frame in which we removed 0 sales rows and tried to train our model. We used various algorithms and got accuracy score around 74%.
We were also curious about the total dataset (including Sales = 0 rows). So we trained another model using various algorithms and we got accuracy near about 92% which is far better than previous model.
So we came to conclusion that removing sales=0 rows actually removes lot of information from dataset as it has 172817 rows which is quite large and therefore we decided not to remove those values. We got our best rmpse score from Random Forest model,we tried taking an optimum parameter so that our model doesnt overfit.



