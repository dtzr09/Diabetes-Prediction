# Diabetes Predictions with KNN, ANN and SVM

This repository aims to predict diabetes based on selected features with three different machine learning models, KNN, ANN and SVM.

The original csv file is taken from https://www.kaggle.com/datasets/pkdarabi/diabetes-dataset-with-18-features/data.

## Aim

To create a machine learning model that can predict whether a user is diabetic or not base on metrics that can be measured at home such as blood pressure and cholestrol levels.

## Workflow

The dataset has been analysed in the `dataset_analysis.ipynb`. 6 columns, `FPG`, `FFPG`, `ALT`, `Tri`, `CCR` and`BUN` as these metrics can only be measured in clinics or hospitals. 

The remaining columns wil then be used for training our ANN, KNN and SVM models.

## Conclusion

Our dataset has non-linear relationships. This is shown in:
1. Comparing the correlation matrix of all the columns with the feature importance by the trained ANN model, we can observe that some fields despite having slightly lower correlation is given a higher feature weight by the model.
2. The SVM classifier performed the best with rbf as its kernel, better than linear kernel. 



