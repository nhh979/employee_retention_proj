# employee_retention_proj
This is the capstone assignment of Google Advance Data Analytics on Coursera.

# The scenario and problem
Analyze the the data collected by the HP department at Salifort Motors and build a model to predict employees who are likely to leave the company.

# Dataset
The dataset can be found [here](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction?select=HR_comma_sep.csv) on Kaggle.
Variable  |Description |
-----|-----|
satisfaction_level|Employee-reported job satisfaction level [0&ndash;1]|
last_evaluation|Score of employee's last performance review [0&ndash;1]|
number_project|Number of projects employee contributes to|
average_monthly_hours|Average number of hours employee worked per month|
time_spend_company|How long the employee has been with the company (years)
Work_accident|Whether or not the employee experienced an accident while at work
left|Whether or not the employee left the company
promotion_last_5years|Whether or not the employee was promoted in the last 5 years
Department|The employee's department
salary|The employee's salary (U.S. dollars)

# Summary
- The baseline XGBoost model achieved AUC of 98.2%, accuracy of 98.2%, precision of 96.3%, recall of 92.7% and f1-score of 94.5% on the test set. These are pretty high scores indicating that the model is strong.
- `avarage_monthly_hours`, `satisfaction_level` and `last_evaluation` are significantly important for the model in predicting employees who are most likely to leave the company.
- Using two sample t-test with a significance level of 5%, we can see that there is no significant difference in average score of the last evalation, whereas there is a statistically significant difference in average monthly working hours and average satisfaction levels between employee who left and who stayed.

![](https://github.com/nhh979/employee_retention_proj/blob/main/images/evaluation_scores.jpg)
![](https://github.com/nhh979/employee_retention_proj/blob/main/images/feature_importance.jpg)
