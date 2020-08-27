# VM Ware-Customer-Engagement

## OBJECTIVE - Improving customer engagement at VMWare through Analytics
1. To find a model with parameters to show the estimates of performance that could be shared with business.
2. Prove that the model could be implemented in the real world so that the business could be convinced of the benifits.
3. Suggest future extensions to this model that the business can incorporate to improve its performance.

## Data and Description
The data consists of 700+ variables from 500+ potential customers from VMWare's web analytics team. As the dataset is confidential, I cannot share the data I received here on GitHub as opensource. However, you can always buy the project from ISB's publication content sharing website.

## Analysis
Dealth with null values and variable data types in order to process the input data in R. Selected significant variables through thorough exploratory analysis. The cleaned the data in R and the code file can be accessed [here](https://github.com/VipanchiKatthula/VMWare-Customer-Engagement/blob/master/code/Project%20Code.R)

## Random Forest Model - Variable selection using Importance
Used the Random Forest model's capability to show the variable importance to identify the significant variables from the variables selected after the exploratory analysis.
![GitHub Logo](/images/RF_model.PNG)

The importance is calculated through the mean decrease in gini index value and below are the top variables that came out significant.
![GitHub Logo](/images/significant_variables.PNG)

## LASSO Regression Model
We built a Lasso regression model using the top 200 variables that came out significant from the Random Forest model. We performed Cross-validation to get the best cost paramater for the LASSO regression.
![GitHub Logo](images/LASSO_Model.PNG) 
