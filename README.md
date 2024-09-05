# Bank_Customer_Churn

## Project Overview
This project focuses on analyzing customer churn using a dataset from a bank. The aim is to identify factors contributing to customer churn and provide actionable insights to improve customer retention strategies. The project utilizes **Python** for data analysis and modeling, and **Power BI** for creating an interactive dashboard.

### Dataset
The dataset used for this analysis is sourced from [Kaggle's Bank Customer Churn Dataset](https://www.kaggle.com/datasets/radheshyamkollipara/bank-customer-churn). It contains various features like customer demographics, account information, and transaction history that are relevant to predicting churn.
## Features

This dataset contains the following features:

1. **RowNumber**: This represents the row number in the dataset and does not affect the customer’s likelihood of leaving the bank.
2. **CustomerId**: A unique identifier for each customer, with no impact on customer churn.
3. **Surname**: The customer's surname, which is irrelevant to their decision to leave the bank.
4. **CreditScore**: A customer’s credit score can influence churn, as those with higher scores are generally less likely to leave the bank.
5. **Geography**: The location of a customer may play a role in their decision to stay or leave the bank.
6. **Gender**: It is worth exploring whether gender impacts a customer's likelihood of leaving the bank.
7. **Age**: This is an important factor, as older customers are often more loyal and less likely to churn compared to younger customers.
8. **Tenure**: This refers to the number of years a customer has been with the bank. Longer-tenured customers are typically more loyal and less likely to leave.
9. **Balance**: A higher account balance may reduce the likelihood of churn, as wealthier customers are less inclined to leave the bank.
10. **NumOfProducts**: The number of products a customer has with the bank can influence churn, as customers with more products may be more invested in the bank's services.
11. **HasCrCard**: Indicates whether a customer owns a credit card. Customers with credit cards tend to be less likely to leave.
12. **IsActiveMember**: Active members are generally more engaged with the bank and less likely to churn.
13. **EstimatedSalary**: Like balance, salary can be an indicator of churn, with lower-income customers being more likely to leave.
14. **Exited**: This column shows whether or not a customer has left the bank (churned).
15. **Complain**: Indicates whether the customer has lodged a complaint, which may affect churn.
16. **Satisfaction Score**: The customer’s satisfaction score for complaint resolution, which may influence their decision to stay or leave.
17. **Card Type**: The type of credit card the customer holds, which may provide insights into their level of engagement with the bank.
18. **Points Earned**: Points accumulated by the customer from using their credit card, which could impact their loyalty to the bank.


- **Number of records**: 10,000
- **Number of features**: 14
- **Target Variable**: `Exited` (1 = Customer has churned, 0 = Customer has not churned)

### Project Steps
1. **Data Preprocessing and Cleaning**: 
   - Handled missing values (if any), outliers, and data types.
   - Categorical variables were encoded using techniques like one-hot encoding.
   - Normalization or scaling was applied where necessary.

2. **Exploratory Data Analysis (EDA)**: 
   - Initial exploration of the dataset to understand feature distributions and correlations.
   - Visualized important trends using matplotlib and seaborn in Python.

3. **Feature Engineering**:
   - Created new features to enhance the prediction model, such as customer tenure, and interaction terms.
   
4. **Modeling and Prediction**:
   - Used **Logistic Regression**, **Decision Trees**, and **Random Forest** models to predict churn.
   - Compared models using evaluation metrics such as **Accuracy**, **Precision**, **Recall**, and **F1-Score**.
   - Hyperparameter tuning was performed to optimize model performance.

5. **Visualization with Power BI**:
   - Created an interactive dashboard in **Power BI** to visualize key metrics such as:
     - Churn rate by customer demographics (gender, age, geography).
     - Customer tenure vs. churn.
     - Comparison of churn by product categories.
   - [Power BI Dashboard Screenshot](./images/powerbi_dashboard_screenshot.png)

### Tools & Technologies
- **Python**:
  - Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn.
- **SQL**:
  - Querying and aggregating data for analysis.
- **Power BI**:
  - Created an interactive dashboard to present findings and insights.
- **Jupyter Notebook**: For performing the analysis and showcasing the code.
- **GitHub**: Version control and project sharing.

### Results
After the analysis, the **Random Forest** model yielded the best results with an accuracy of 85%. Key findings from the analysis include:
- **Senior Citizens** are more likely to churn.
- **Customers with higher balances** are less likely to churn, whereas **customers with higher tenure** tend to stay.
- **Churn is significantly higher among customers who do not have a credit card.**

### Power BI Dashboard
An interactive dashboard was created using Power BI to visualize the key metrics and trends related to customer churn. You can view the insights by downloading the `.pbix` file and opening it in Power BI.

