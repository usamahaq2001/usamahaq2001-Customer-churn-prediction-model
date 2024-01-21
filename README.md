# usamahaq2001-Customer-churn-prediction-model
In this repository I have added my project "Customer Churn Prediction Model" including EDA.

## Scenario

Our client is a major gas and electricity utility that supplies to small and medium sized enterprises.\
The energy market has had a lot of change in recent years and there are more options than ever for customers to choose from.\
Our clients are concerned about their customers leaving for better offers from other energy providers. When a customer leaves to use another service provider, this is called churn.\
This is becoming a big issue for our client and they have engaged to help diagnose the reason why their customers are churning.

## Hypothesis

Client discussed some potential reasons for this churn, one being how “sensitive” the price is. In other words, how much is price a factor in a customer’s choice to stay with or leave ?

## EDA

The visualization shows how many companies churned vs. how many companies did not churn. We can see from this that the churn rate is approximately 10%. This is actually a very good churn rate, the closer the rate is to 0%, the better.\
The next series of visualizations were created in an attempt to try and dive deeper into how churn changes based on other factors (using other columns). This is useful for us to investigate because it may help us to understand factors that drive churn.\
In the notebook we visualize churn vs. sales channel, contract type, number of products, number of years and origin/contract offer.\
For example:\
We see that for sales channel, there are some sales channels that yield customers churning but there are also other sales channels that have no customers churning.\
For contract type, we see quite an even split for customers churning. This is interesting because this may suggest that contract type is not a driving factor towards churn rate.\
Additionally, for some columns their distributions with churn rate included. This is useful for us to understand because based on the distribution of a column, this could affect our feature engineering later.\
We look at the distribution of consumption, subscribed power and forecast in the notebook. \
For example:\
We notice that the distribution of consumption is very skewed, this is called a positive skew since it is biased towards lower values on the x axis.\
This is interesting because you may decide to treat this column to reduce the skewness later on during feature engineering. But also because we may want to visualize if there are any outliers within this column. \
To investigate outliers, we use a boxplot. From the boxplot we can see that with the column as it is there are definitely some outliers. Once again this is interesting because we may choose to remove some of these outliers later.

## Model Building

We have performed the feature engineering on the data set that includes rescaling some features, deducing some of the features based on their predictive powers, encoding the categorical features and lastly applying the models and evaluating their performance with the hepl of different metrics.

## Finding 

To answer our hypothesis:\
"How sensitive the feature price is for the customer's churn"?\
By analyzing the feature importance after applying classification model, we can clearly see that price is not very much of the important feature for the churn of the customer's.
