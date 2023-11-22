# Python Project- Home Loan Eligibility Prediction
## Business Problem 
Urban Finance Ltd specialises in all types of home loans. In recent years, their client base has grown significantly, and they want to automate the loan eligibility process. Based on the customer details that were submitted online. As a data scientist working for Urban Finance Ltd, I’m responsible for building Machine learning to find eligible customers.
## Data Preparation
Raw Data was given by Urban Finance. I filled null values with either median or mode, Income and loan amount were transformed into Logarithm. Dropped Loan ID as unrelated data. Dummy variables were introduced to form a regression equation. Replaced “Y” with “1”, and “N” with “0” in loan status for modeling purposes. We now have 12 independent variables and one target variable, Loan Status. 
