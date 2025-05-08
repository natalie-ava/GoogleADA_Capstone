# Model Results

This folder contains output files and evaluation metrics from the logistic regression model used to predict employee departures.

## Files Included

- [`classification_report.txt`](./classification_report.txt): A detailed summary of model performance, including precision, recall, and F1-score for both classes.
- [`confusion_matrix.pdf`](https://github.com/natalie-ava/GoogleADA_Capstone/blob/main/images/confusionmatrix.pdf): Visual representation of model predictions compared to actual values. The confusion matrix helps illustrate where the model performed well and where it made errors.

## Summary

The model achieved an accuracy of 84%, with high precision for predicting who stayed. However, recall for employees who left was lower (23%), which suggests the model misses a number of at-risk individuals. The confusion matrix and classification report provide valuable context for refining the model in future iterations.

## Next Steps

Further tuning, alternative models (such as Random Forest or Gradient Boosting), and additional feature engineering may improve recall while maintaining accuracy.
