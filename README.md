# Python Project- Home Loan Eligibility Prediction
## Business Problem 
Urban Finance Ltd specialises in all types of home loans. In recent years, their client base has grown significantly, and they want to automate the loan eligibility process. Based on the customer details that were submitted online. As a data scientist working for Urban Finance Ltd, I’m responsible for building Machine learning to find eligible customers.
## Data Preparation
Raw Data was given by Urban Finance. I filled null values with either median or mode, Income and loan amount were transformed into Logarithm. Dropped Loan ID as unrelated data. Dummy variables were introduced to form a regression equation. Replaced “Y” with “1”, and “N” with “0” in loan status for modeling purposes. We now have 12 independent variables and one target variable, Loan Status. 

![Picture1](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/f04bbe01-b1de-444e-8212-2c6d77b4cb85)
![Picture2](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/9b75314c-e406-452e-9f4d-479c50cd27fd)

## Data Analysis and Visulisation 
Overall we can see most applicants' income between $10,000-$40,000 per year, and Almost 70% of the applicants that applied for home loan in Urban Finance Ltd have been approved.

![Picture3](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/9d53c2d4-7f23-480a-9009-a548b0e326e9)
![Picture4](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/fb540773-6f90-4e5c-9837-ac626b954c75)

Loan amount and Applicant Income have the highest correlation, and Credit history and Loan status have the highest correlation. 

![Picture5](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/70ebe396-6daf-47a1-a8ca-361cc6f84f82)

Credit score plays a big part in home loan approval. Almost 80% of applicants with good credit have been approved for a home loan, About 70% of applicants with bad credit have been declined for a home loan

![Picture6](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/dd9ccd3b-43aa-4c54-875f-171d397f6712)

From the Data, the approval rate does not change much When Incomes are average or higher. However, 60% of the low-income group’s loan application has been declined 
(Low Income 0-$2,500 per month, Average Income $2,500-$4,000 per month ,High Income $4,000-$6,000, Very High Income $6,000-$81,000)

![Picture7](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/00c5bb65-07b9-4a58-a64f-700eb98707d3)

### Logistic Regression Model
I use Logistic Regression Model to predict the category dependent variable “Loan_Status”. First split the data with 80% train data and 20 % test data. Fit into Logistic Regression model, and scored about 76% the model's accuracy. 

![Picture8](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/cd544d5a-5b47-48c7-b50a-ba6496222ec4)
![Picture9](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/5ed34d31-31c1-452f-8afc-6debfcca6938)

### Decision Tree Model 
I then used Decision Tree Model, and initially achieved a model accuracy of 65%. Applied Decision Tree Parameter Tuning. Random Search model achieved model accuracy of 73.1%. Grid Search Model achieved model accuracy of 78.9%. accuracy of the model has significantly increased by 13% by using the best parameter.

![Picture10](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/264a059d-e4a1-41b5-ae0f-ac39cb4a9c46)
![Picture11](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/041837ab-e657-4ad3-8a15-3ca83d03f3c2)

### Random Forrest Model
Random Forrest Model achieved accuracy score of 69% . Hyperparameter Tuning with Grid Search Accuracy score Jump up to 77.2%. Model also suggests most Important feature is Credit History

![Picture12](https://github.com/dandai509/Python-Project-Supervised-Machine-Learning/assets/106848444/afae8612-d1ff-40b8-bbab-15ae8596cfa7)

## Summary
Supervised Macchine learning model is built to automate loan approval process for Urban Finance Ltd. Decision Tree model with Hyperparameter Tunning of Grid search has the best accuracy of 79%. Variety factors affect loan approval, Credit history, total income,  property area, and loan amount as being top 4. People with high income and a good credit history are more likely to get Home Loan approved.
Urban Finance can now gather supplication information from its website and use this model to filter applications. The model will automatically approve or decline applications depending on the data given. This model has saved much time compared to manually selecting the application to check and prove. it improved the productivity of the company significantly.






