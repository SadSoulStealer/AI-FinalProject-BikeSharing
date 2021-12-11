# AI Final Project: PyCaret Analysis With Bike Sharing Dataset

# Abstract
Bike Sharing is a rising trend when it comes to transportation around larger cities. Due to how global warming is rapidly affecting our lives everyday, the move to bikes in order to lower our emissions is a very good idea. However, many cities are against these services in place and actively aim to kick them out as they believe no one is really using them. This project aims to use various machine learning algorithms through the PyCaret library in order to create an accurate model to predict and demonstrate how well bike sharing services are actually doing. This was performed on the UCI Bike Sharing Dataset collected by the Laboratory of Artificial Intelligence and Decision Support in late 2013. Results from our tests show that the Light Gradient Boosting Machine, Extra Trees, and Random Forest classifiers performed very highly by the performance metrics we chose to analyze. After tuning, the Light Gradient Boosting Machine model provided us with the highest level of prediction we could achieve by looking at our R2 and RMSE. This model performed very well when tested on unseen data.

# Explanation
To see a short explanation of the project, check out [this video](https://youtu.be/XrZGz14gUds)

# Feature Engineering
| Feature | Category |
| ------------- | ------------- |
| season  | Categorical |
| yr | Categorical  |
| mnth | Categorical  |
| hr  | Numeric |
| holiday | Categorical |
| weekday  | Categorical  |
| workingday  | Categorical  |
| weathersit | Categorical |
| temp  | Numeric | 
| atemp  | Numeric |
| hum  | Numeric  |
| windspeed | Numeric |
| cnt  | Label | 

I dropped the columns for dteday, instant, casual, registered. I dropped dteday because the date provides not value in the model we were creating. Next, I dropped casual and registered as we already have cnt as our target variable which encompasses the total of those two vatiable. Finally, I dropped instant as it provides no value to our model.

# Performance Metrics
In terms of the performance metrics, I used is R2 and RMSE. I used RMSE because it is measured in the same units as the response variable. For R2, I chose this because I think variation is important in terms of comparing models.
