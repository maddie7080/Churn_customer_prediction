# Churn customer Prediction model.

## Problem Statement
The client is one of the famous bank from Mozambique.They need to predict the churn customer by using the historical data available to them.Basically it was a classification problem between active and churn customer.Click through rate has to be increased by recommending him/her with right product so that the customer could continue his services with the bank.
## Approach:
1. Build the project pipeline by engaging with SME from the bank.
2. Gaining the knowledge about the business domain.
3. Collecting the data and pre-processinng it for further step.
4. EDA has been done on historical data to plot the observations.
5. Choosing the right ML algorithm and training the data upon it.
6. Plotting the result by using test data and checking through it by cross validation techinques. 
7. Finally we came up with web app which was build by using sagemaker studio as prototype to showcase the result.
## Observations from eploratory data analysis:
1. Average customer month income is quite high for churn customer as compared to active customer.
2. The average male customer is quite acitve as compared to female customer also the male churn customer  is quite high compared to female churn customer.
3. Mostly the active customer are single one and the second most active customers are married one       similalry the churn customer are mostly contributed by single and married      as compared to other customer marital status.¶
4. If the average transaction per season are lesser than 20, then the customer tends to be a churn customer.¶
5. The debit amount for churn customer is about 3 times lesser than of the active customers. The debit amount for churn customers lies between 20,000 to 1,00,000.
6. Total number of credit transactions done by churn customers is around 2 to 3 as opposed to 8 or >8 by active customers
7. Total credit amount for churn customer lies in the range 20,000 to 60,000 as opposed to active customers with avg credit amount of 3.5 lakh or greater than 3.5 lakh.
8. Total debit transactions is about 4 to 5 times lesser in churn customer.
## Challenges
1. Banks takes longer time to collecting the enough data to perform analysis on issue as there is question of reliability of the data.
2. Getting right significant column which could be the unique features to indetify the churn customer.So we used Cramer correlation.
3. Data were highly imbalanced as there was only 1200 Bank customer records about which 82% were active customer and only 18% were churn customer, this could lead to problem of      overfitting.But this was handled by normalizing the data.
4. Choosing right ML solution so we kept in incremental approach, by using different algorithms but Random forest classifier tends to be the perefect algorithm with the best          accuracy which is around 84%.
## Outcome
The prediction model is build to identify the churn customer and active customer proactively and the customer were recommended with right product to continue his sevices with bank this lead to significant increase in ROI in terms of CTR by 15%-20%.
