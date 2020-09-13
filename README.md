# Identification-of-Personal-Loan-Acceptors-R

Problem statement: The Universal Bank is interested in growing it's base of asset customers to bring in more loan business. They are planning to run a marketing campaign to convert liability customers to asset customers. Given this type of targeted marketing, the goal of my analysis is to analyze customer behaviour in terms of various attributes and look for a combination of factors that make a customer more likely to accept a personal loan.

The predictive model that I have used in this case is Logistic Regression Classifier. The dataset constitutes information about 5000 customers. Following is a description of the attributes that I have used to study customer behaviour.

Age- Customer’s age in completed years

Experience- Number of years of professional experience

Income- Annual income of the customer ($000s)

Family- Size Family size of the customer

CCAvg- Average spending on credit cards per month ($000s)

Education- Education Level. 1: Undergrad; 2: Graduate; 3: Advanced/Professional

Mortgage- Value of house mortgage if any ($000s)

Securities- Account Coded as 1 if customer has securities account with bank

CD Account- Coded as 1 if customer has certificate of deposit (CD) account with bank

Online Banking- Coded as 1 if customer uses Internet banking facilities

Credit Card- Coded as 1 if customer uses credit card issued by Universal Bank



If we look at the summary of the logistic regression model, where the independent varibales are all the features described above, and the target variable is whether or not the customer will accept a personal loan offer ( 1: accept 0: reject), we find that there are 7 attributes that are statistically significant in the order - Income, Family size, Education level(graduate), Education level(professional), credit card average, CD Account and Credit Card.

How do I decide these variables are statistically significant? 
I looked at the p-values associated with coefficients of attributes in the model summary.

confidence level = (1 - p-value) X 100

implies, smaller the p-value, greater will be the confidence level for that variable.


Also, for evaluating the model performance, take a look at the confusion matrix. Metrics like accuracy and error rate can be calculated from there.
