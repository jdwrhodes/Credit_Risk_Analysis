# Machine Learning

## Overview
The purpose of this project was to analyze the predictive capability of different machine learning algorithms regarding credit risk.

## Results
Six different machine learning algorithms across four different categories were analyzed with the results below, specifically highlighting the accuracy, precision, and recall scores.

### Oversampling
- Naive Random Oversampling (NRO):
  - Accuracy score was 0.649, meaning the model predicted the correct classification of Low or High credit risk 64.9% of the time.
  - The Precision score was 0.01, or 1%, for high risk and 1.00, or 100%, for low risk. Precision indicates the reliability of a classification, here for it is vey very poor at 1% for high. But it is perfect at 100% for low risk classification prediction.
  - The Recall score was 0.73, 73%, for high risk prediction and 0.57, or 57% for low risk. Recall indicates how many were actually correctly classified in each category. For high it correctly classified high risk 73% of the time, whereas it only correctly classified low risk 57% of the time.

![Naive Random Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/naive_random_acc_score.png 'Naive Random Accuracy Score')
![Naive Random Oversampling](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/naive_random_report.png 'Naive Random Oversampling')
- SMOTE: 
  - Accuracy score here was 0.658, or 65.8% correct classification.
  - Precision was like the Naive Random Oversample above (NRO), at 0.01 for high risk and 1.00 for low risk.
  - For high risk the Recall score was 10% lower than the NRO algorithm, at 0.63, 63%. Low risk was 11% higher at 0.68, 68%.

![SMOTE Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smote_acc_score.png 'SMOTE Accuracy Score')
![SMOTE](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smote_report.png 'SMOTE')

### Undersampling
- Cluster Centroids: 
  - Accuracy score
  - Precision
  - Recall

![Cluster Centroids Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/cluster_centroid_acc_score.png 'Cluster Accuracy Score')
![Cluster Centroids](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/cluster_centroid_report.png 'Cluster Centroids')

### Over and Undersampling Combination
- SMOTEENN: 
  - Accuracy score
  - Precision
  - Recall

![SMOTEENN Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smoteenn_acc_score.png 'SMOTEENN Acurracy Score')
![SMOTEENN](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smoteenn_report.png 'SMOTEENN')

### Ensemble
- Balanced Random Forest Classifier: 
  - Accuracy score
  - Precision
  - Recall

![Balanced Random Forest Classifier Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/balanced_rf_acc_score.png 'Balanced Random Forest Classifier Accuracy Score')
![Balanced Random Forest Classifier](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/balanced_rf_report.png 'Balanced Random Forest Classifier')

- Easy Ensemble Classifier: 
  - Accuracy score
  - Precision
  - Recall

![Easy Ensemble Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/easy_ensemble_acc_score.png 'Easy Ensemble Accuracy Score')
![Easy Ensemble Classifier](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/easy_ensemble_report.png 'Easy Ensemble Classifier')

## Summary


Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
