Customer Churn Prediction

Problem statement

In business, churn is defined as a measure when customers leave company or purchase process during agiven period. Churn prediction, is the process of using machine learning algorithms to identify whichcustomers are likely to churn in the future. This is important for companies because it is usually moreexpensive to acquire new customers than to retain existing ones. It can help companies focus on retainingcustomers who are at risk of leaving the company. The E-commerce project is conducted to respond to thestatement “Which customers are likely to churn during the purchase process?” using Machine Learning.

Data Definition

Session Count (Each time an user initiates a session, a session counter increments for that user)
Event Count (Number of times the event was triggered)
Closed Session Event Count (Number of times the session was closed )
Open Session Event Count (Number of times the customer logged into the system)
Quest Completed Event Count ( Whatever the user was searching they found )
Store Purchase Event Count ( Number of times the item was purchased)
Active Days( Number of days the session was active )
Session Length Minutes ( Session length is typically defined as the amount of time the app is in front of theuser )

Insights

The active days of customers range from 1 to 60 days. Around 38 % customers churn having low activedays. As the active days increase the retention rate increases significantly.
Around 65% customers have session lengths (min) of 0 to 390 minutes, out of which around 42 % churned,while only 23% stays. As the session length tends to increase, although the number of customersdecreases, retention rate increases.
Around 75% of customers have either 0,1 or 2 store purchase event count, with around 43 % churn rateand 32 % stay rate. As the store purchase event count increase the churn rate drops to just 3 %.
Customers with lower session count tend to churn more, compared to customers with higher season count.
Event count with highest number of customer is in bracket 0 to 600, out of which 45 % churn, while only 25% stay. Also as the event count increases the stay rate increase significantly.
The interpretation of open session event count and closed session event count is same. Around 65 % withlowest (0 to 60) closed and open session event count have highest churn rate. As the open and closesession count increase the number of customers reduces significantly. There are few customers with veryhigh values, out of which 16 % stay and only 2 % churn.

Modeling

Decision Tree, Random Forest, Logistics Regression, and Linear Regression are preferred tools for thisproblem. Model performance will be conducted using Accuracy, Sensitivity, Specificity, Precision and F1-score.
For the purpose of this problem, the model is expected to identify as many customers who are likely toChurn as possible. Hence, Sensitivity which measures the ratio between how much are correctly identifiedas churn to how much are actually churn, is set to be the main measure.
Model Performance
The Logistics Regression model yields the relatively good result across Accuracy, Sensitivity, andSpecificity in both train and test data. This is the best model for predicting churn with sensitivity for trainand test data being 97 % and 96 % respectively. Also logistic regression has a good accuracy score of 68% for train data and 67 % for test data.
Logistic Regression will be the chosen model for implementation as it yields the highest Sensitivity andgreat insights into feature significance.

Recommendations

Based on the outcomes produced by the Logistic Regression model, the management team is recommended toconsider a number of approaches to manage customers with high likelihood of churn, which include:
Incentives that encourage customers to stay for longer times on the applications so the churn rate couldreduce. The company may consider incentives for those who used the application for a certain number oftime. This can be applied to campaigns that encourage customers to get to know the benefits of the app.For example, 5% discount of total premium if a customer used the app daily for a week. The revenueforgone in form of discount should outweigh the cost of churn to ensure the feasibility of the initiative.
Attractive offers for new customers, and those in the high churn propensity list.
If the company's strategy favors customer retention, stricter risk analysis and management should be inplace.
The customer persona also helps to identify customers with high chance of churn when they use theapplication. The company may monitor their online activity closely and identify the probable causes newcustomers close the application.
The company could work to provide more features, better UI and user experience to its customers.
