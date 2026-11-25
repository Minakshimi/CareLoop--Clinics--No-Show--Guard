
# Patient Appointment No-Show Prediction

## Project Summary

Part 1: Analysed appointment data to understand patterns associated with patient no-shows.

Part 2: Prepared the dataset and created features for predicting missed appointments.

Part 3: Built a Balanced Logistic Regression model with 68.18% test accuracy and 0.742 ROC-AUC.

Part 4: Used Gemini to analyse appointment notes and identify reasons for missed appointments.

## Business Recommendation

The clinic should use the no-show prediction model to identify patients who may need additional reminders. The model identified 30 of 44 actual no-shows in the test dataset, giving a recall of 68%. However, its precision was 38%, meaning many patients flagged as high-risk would still attend. The clinic should consider the cost of unnecessary reminders and use the model as a support tool rather than relying on it as a definitive prediction.

## Limitations

1. Only 10 notes were analysed using the GenAI model, so they cannot represent all clinic-wide reasons for missed appointments.
2. The model was trained on data from before the train-test split, so its evaluation may not represent future performance.
3. The same patient may appear in both the training and test datasets.
4. The train-test split was random rather than based on appointment dates.
5. The data is observational, so the associations found do not establish causation.
