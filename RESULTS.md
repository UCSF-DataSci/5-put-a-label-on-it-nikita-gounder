# Assignment 5: Health Data Classification Results

This file contains your manual interpretations and analysis of the model results from the different parts of the assignment.

## Part 1: Logistic Regression on Imbalanced Data

### Interpretation of Results

In this section, provide your interpretation of the Logistic Regression model's performance on the imbalanced dataset. Consider:

- Which metric performed best and why?
- Which metric performed worst and why?
- How much did the class imbalance affect the results?
- What does the confusion matrix tell you about the model's predictions?

*In the Logistic Regression model on imblanaced data, accuracy was the best metric at 0.9168 while recall was the worst at 0.3007.The high accuracy is exaggerated because the class imbalance and low recall means the model couldn't identify a lot of true positive cases. The confusion matrix shows the model predicted the negative class pretty good but missed true positive cases. This means the model was biased because of the imbalanced data. *

## Part 2: Tree-Based Models with Time Series Features

### Comparison of Random Forest and XGBoost

In this section, compare the performance of the Random Forest and XGBoost models:

- Which model performed better according to AUC score?
- Why might one model outperform the other on this dataset?
- How did the addition of time-series features (rolling mean and standard deviation) affect model performance?

*According to the AUC score, the XGBoost model did better at 0.9965. In xgboost, gradient boosting probably allows for better fit than random forest. The addition of time-series features like rolling mean and rolling standard deviations for heart rate helped the models have better fit.*

## Part 3: Logistic Regression with Balanced Data

### Improvement Analysis

In this section, analyze the improvements gained by addressing class imbalance:

- Which metrics showed the most significant improvement?
- Which metrics showed the least improvement?
- Why might some metrics improve more than others?
- What does this tell you about the importance of addressing class imbalance?

*In the Logistic Regression model on balanaced data, recall was the best metric at 0.8392 while precision was the worst at 0.3200.Recall went from the worst to best metric comparing to the previous unbalanced model. There is now better prediciton of posiitve classes. The confusion matrix is better with more true positive cases. Addressing class imbalance is important to have more accurate metrics that are not biased towards classes. *

## Overall Conclusions

Summarize your key findings from all three parts of the assignment:

- What were the most important factors affecting model performance?
- Which techniques provided the most significant improvements?
- What would you recommend for future modeling of this dataset?

*Overall, the most important features for mdoel performance is addressing class imbalance and making sure the features are formatted correctly (time-series). Balancing the classes showed the most improvement. In future modeling of this datasets, I reccomend class-balancing techniques (SMOTE), to personalize features to the data, and choose the best model for the data (randomforest v logistic v xgboost).*