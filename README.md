# Google's Advanced Data Analytics Capstone: Predicting Employee Turnover

This project explores employee departure patterns at a mid-sized company using logistic regression. The primary goal is to identify key factors that influence whether an employee leaves and to build a predictive model that supports Human Resources in proactive decision-making.

## Project Objectives

- Perform exploratory data analysis (EDA) to uncover trends related to satisfaction, workload, and employee departure
- Build and evaluate a logistic regression model to predict whether an employee is likely to leave the company
- Interpret model results and generate actionable insights for business strategy
- Provide practical recommendations to improve employee retention

## Dataset

- Source: [Kaggle HR Analytics Dataset](https://www.kaggle.com/datasets/mfaisalqureshi/hr-analytics-and-job-prediction)
- The dataset contains 15,000 employee records and the following features:

| Variable               | Description                                                              |
|------------------------|---------------------------------------------------------------------------|
| satisfaction_level     | Employee-reported job satisfaction level (range: 0 to 1)                 |
| last_evaluation        | Score of the employee's last performance review (range: 0 to 1)          |
| number_project         | Number of projects the employee contributes to                           |
| average_monthly_hours  | Average number of hours the employee worked per month                    |
| time_spend_company     | Number of years the employee has been with the company                   |
| Work_accident          | Indicates whether the employee experienced a work-related accident       |
| left                   | Indicates whether the employee left the company (target variable)        |
| promotion_last_5years  | Indicates whether the employee was promoted in the last 5 years          |
| Department             | The employee's department (e.g., sales, technical, support)              |
| salary                 | The employee's salary level (e.g., low, medium, high)                    |


## Technologies Used

- Python 
- Pandas for data manipulation  
- Seaborn and Matplotlib for data visualization  
- Scikit-learn for modeling and evaluation

## Results and Model Evaluation
The confusion matrix below shows the performance of the logistic regression model on the test set:

|                | Predicted: Stayed (0) | Predicted: Left (1) |
|----------------|------------------------|----------------------|
| Actual: Stayed (0) | 1933                   | 65                   |
| Actual: Left (1)   | 310                    | 91                   |

- **Accuracy**: 84%  
- **Precision (left = 1)**: 0.58  
- **Recall (left = 1)**: 0.23  
- **F1-score (left = 1)**: 0.33

## Key Findings

- Low satisfaction and longer work hours are the strongest predictors of employee departures
- The logistic regression model achieved an overall accuracy of 84%
- Recall for identifying employees who left was 23%, indicating the model misses some high-risk individuals
- The F1-score reflects a moderate balance of precision and recall
- AUC scores suggest that the model ranks employee risk reasonably well but could be improved with additional features

## Recommendations

- Monitor employee satisfaction and workload levels as part of routine HR assessments
- Implement targeted check-ins with high-tenure employees or those at risk of burnout
- Use the model as a decision-support tool rather than a standalone solution to ensure fair and ethical outcomes

## Next Steps

- Incorporate more features such as promotion history, department-level trends, and feedback data
- Test alternative models such as Random Forest or XGBoost to improve predictive performance
- Use cross-validation and rebalancing strategies to address class imbalance and strengthen recall

## Ethical Considerations

- Employee data is used solely to support engagement and retention strategies
- Predictions should guide supportive interventions, not punitive action
- Continuous review of model fairness and bias is recommended to ensure responsible application

## Repository Contents

- [`NHuang_GoogleADA_Capstone.ipynb`](https://github.com/natalie-ava/GoogleADA_Capstone/blob/main/NHuang_GoogleADA_Capstone.ipynb): Final notebook containing exploratory and visual analysis, modeling, and results
- [`data/`]: original and leaned dataset used in this project
- [`images/`]: Visualizations including confusion matrix and correlation heatmaps
- [`results/`]: Model outputs and reports
