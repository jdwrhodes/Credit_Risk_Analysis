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

![Naive Random Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/naive_random_acc_score.png 'Naive Random Accuracy Score') ![Naive Random Oversampling](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/naive_random_report.png 'Naive Random Oversampling')
- SMOTE: 
  - Accuracy score here was 0.658, or 65.8% correct classification.
  - Precision was like the Naive Random Oversample above (NRO), at 0.01 for high risk and 1.00 for low risk.
  - For high risk the Recall score was 10% lower than the NRO algorithm, at 0.63, 63%. Low risk was 11% higher at 0.68, 68%.

![SMOTE Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smote_acc_score.png 'SMOTE Accuracy Score') ![SMOTE](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smote_report.png 'SMOTE')

### Undersampling
- Cluster Centroids (CC): 
  - Accuracy score was 0.544, 54.4%, lower than NRO and SMOTE.
  - Precision was the same again at 0.01, 1%, for high risk and 1.00, 100%, for low risk.
  - Recall for high risk landed between NRO and SMOTE at 0.69, 69%, but low risk was the lowest result so far at 0.40, 40%.

![Cluster Centroids Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/cluster_centroid_acc_score.png 'Cluster Accuracy Score') ![Cluster Centroids](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/cluster_centroid_report.png 'Cluster Centroids')

### Over and Undersampling Combination
- SMOTEENN: 
  - Accuracy score was 0.662, 66.2%, which is the highest out of all the algorithms so far.
  - Like the previous algorithms, the Precision score was the same at 0.01, 1%, for high risk. It was also 1.00, 100%, for low risk.
  - The Recall score for high risk raised the bar to 0.78, 78%, whereas low risk is second from the bottom at 0.54, 54%.

![SMOTEENN Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smoteenn_acc_score.png 'SMOTEENN Acurracy Score') ![SMOTEENN](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/smoteenn_report.png 'SMOTEENN')

### Ensemble
- Balanced Random Forest Classifier (BRF): 
  - Accuracy score of 0.789, 78.9%, was achieved, the second highest out of all the algorithms.
  - Precision score for high risk was finally raised to 0.03, 3%. Low risk stays the same as the other algorithms at 1.00, 100%.
  - Recall score for high risk drops to 0.70, 70%, though low risk actually has increased to 0.87, 87%, second highest among the algorithms.

![Balanced Random Forest Classifier Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/balanced_rf_acc_score.png 'Balanced Random Forest Classifier Accuracy Score') ![Balanced Random Forest Classifier](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/balanced_rf_report.png 'Balanced Random Forest Classifier')

- Easy Ensemble Classifier (EE): 
  - Accuracy score is the highest among all the algorithms at 0.931, 93.1%.
  - Precision score for high risk is 0.09. 9%, again the highest. Low risk score stays the same at 1.00, 100%.
  - Recall score for both categories is the highest, 0.92, 92%, for high risk, and 0.94, 94%, for low risk.

![Easy Ensemble Accuracy Score](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/easy_ensemble_acc_score.png 'Easy Ensemble Accuracy Score') ![Easy Ensemble Classifier](https://raw.githubusercontent.com/jdwrhodes/Credit_Risk_Analysis/main/Module-17-Challenge/resources/easy_ensemble_report.png 'Easy Ensemble Classifier')

## Summary

Out of all the models, the best performer was the Easy Ensemble Classifer followed by the Balanced Random Forest Classifier. Both of these belong to the Ensemble category of classifiers. Personally I would use the Easy Ensemble classifier as it was able to raise it's high risk Precision score (0.09) further than any other model while also achieving a Recall score of over 90% for both low and high risk. Though more iteration and training with different datasets could improve the model's accuracy even further.
