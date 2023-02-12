# PREDICTION OF CHURN IN SYRIATEL TELECOM <br>
![Main image](https://www.itnewsafrica.com/wp-content/uploads/2020/05/Telecoms.jpg)

## Introduction <br>
For a telecom company, it is important to know what factors contribute to the people leaving as to understand this would help your business to identify it's weaknesses and find ways to deal or combat the issues it has. <br>
This project aims to predict churn by using other factors and using logistical regression.

## Business Understanding.
The telecommunication company is losing customers every month and with everyone wanting to know why there seem to be losing customers they created a Dataset with the target to identify the people that left and stayed while looking for factors that have contributed to their departure.
They also need to know the at risk of leaving groups in order to put some effort into trying to keep them as customers.

## Research Question.
The main goal of the project was to use Data Analysis to identify the factors that lead to churning.

## Objectives.
Perform Exploratory Data Analysis of the dataset to understand each variable, and their relationship among each other, and to the target the churn
*To identify the variables affecting churn.<br>
*To create a model that relates churn with variables <br>
*Predict the values <br>
*Evaluating our model on how well these it can predict churn.<br>
*Come up with conclusions and recommendations.<br> 
# Data

## Data Preparation.
The Dataset was sourced from kagle but was downloaded and opened locally and stored in a CSV file and loaded into Python using the pandas library.The Dataset was cleaned by checking for null values and duplicates.The Dataset types for each column were checked. The minutes ,charges and number of calls were all added in to make the total minutes, total charges and total calls for better analysis.<br>
the data was found here [Dataset](https://www.kaggle.com/datasets/becksddf/churn-in-telecoms-dataset/download?datasetVersionNumber=1)
## Exploratory Data Analysis
The Data was analysed based on relationships fore seen and with a number of columns being binned to see rate of churn with each oof the specific groups.
![total charges_countplot](https://user-images.githubusercontent.com/117269915/218333029-9e34fe9d-a5b1-4d16-8448-e96db44e13fa.png)

With churn being a binary there were alot of catplots used to compare continuous variables and crosstabs to compare Churn with other categorical variables.<br>

The categorical variables were encoded usin One-Hot encoding 


## Data interpretation
A correlation heatmap between these columns in the Dataframe were compared to churn<br>
![correlation_heatmap](https://user-images.githubusercontent.com/117269915/218333045-c132788e-27af-466c-afab-94bcb4868ce7.png)



## Modeling.
The Data was split into test and Train with a Random_state of 42 and the test percentage was left to Default meaning 75% would be used to train and the training 25% would be used to test/validate. The target variable churn was set to y and the rest of the dataset was set to X 
We were able to do a logistic regression on the Dataset since the Target variable was binary(meaning only 2 options were available true or false) and came up with an accuracy score which was a little lower than expected which meant it was under fitted therefore meaning using (nsert mdel) which then made it higher but with adding a few Hyperparameter is to improve the accuracy score to a more acceptable place.

## CONCLUSIONS
*The customers charged above 40 dollars are at very high risk of churning
*The customers who have higher customer care calls above 4 calls are very likely to churn.
*the highest churn percentage (26.4%) was noticed in CA against the national aVG of (AVG_NAT)
*Account length doesnt reduce churn rate.
## Recomendations/further research
*Research why CA,tx and MD percentage for churn is that high (for example CA as to why the churn is 24.X% while the average national is 14% )
*Market and promote international plan as most of the people who receive international calls have no international plan
*Get more information on your customers like Age,gender to understand more demographics of your customers
*Customers with more than 3 cutomer care calls should have access to a managers or people of authority.



