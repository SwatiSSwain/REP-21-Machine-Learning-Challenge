Machine Learning Challenge - Exoplanets Exploration

Analysis
Model-1 SVM

For this model, the first step was to decide what fields to use in the model. And then assign X and y by scaling the data using Max Scaler. The next step was to perform split data to get train and test data for the model.

Below are the scores for the SVN model:
Training Data Score: 0.8916650772458516
Testing Data Score: 0.8878718535469108

GridSearchCV was used to tune the model, however changing the grid parameters C and gamma didn't get any score improvement.

Below is the Classification Report:

                    precision    recall      f1-score   support

     Confirmed       0.81      0.70      0.75       411
False Positive       0.78      0.84      0.81       484
     Candidate       0.98      1.00      0.99       853

      accuracy                           0.89      1748
     macro avg       0.86      0.85      0.85      1748
  weighted avg       0.88      0.89      0.88      1748



Model-2 Logistic Regression

For this model, the first step was to decide what fields to use in the model. And then assign X and y by scaling the data using Max Scaler. The next step was to perform split data to get train and test data for the model.

Below are the scores for the Logistic Regression model:
Training Data Score: 0.8903299637612054
Testing Data Score: 0.8832951945080092

GridSearchCV was used to tune the model, however changing the grid parameters C and and increasing the number of iterations max_iter didn't get any score improvement.

Below is the Classification Report:

                    precision    recall  f1-score   support

     Confirmed       0.79      0.72      0.75       411
False Positive       0.78      0.83      0.80       484
     Candidate       0.99      0.99      0.99       853

      accuracy                           0.88      1748
     macro avg       0.85      0.85      0.85      1748
  weighted avg       0.88      0.88      0.88      1748

Conclusion:
The two models, SVM and LogisticRegression didn't have any significant difference and hyperparameters tuning didn't help the score. In conclusion, SVM model was sligtly better than Logistic Regression.