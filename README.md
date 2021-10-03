# Credit_Risk_Analysis

## Overview
 
## Resources
- Software: Python 3.7.10, VsCode 1.60.2
- The data was provided via csv file (LoanStats_2019Q1.csv).

## Results
- Oversampling
	- Oversampling Imbalanced Classification Report
	
	![Oversampling](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/Oversampling.png)

	- The balanced accuracy for the Oversampling model is 63.34%. The precision score is very low at 1%. The recall score is 59% which is also low.
	
- SMOTE Oversampling
	- SMOTE Oversampling Imbalanced Classification Report
	
	![SMOTE Oversampling](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/SMOTE_Oversampling.png)

	- The balanced accuracy for the SMOTE Oversampling model is 63.15%, similar to the Oversampling accuracy. The precision and recall is also nearly identical to the Oversampling model.
	
- Undersampling
	- Undersampling Imbalanced Classification Report
	
	![Undersampling](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/Undersampling.png)

	- The balanced accuracy for the Undersampling model is 62.03%, which is least accurate of the 6 models. This model also have the lowest precision and recall figures. 
	
- Combination (Over and Under) Sampling
	- Combination (Over and Under) Sampling Imbalanced Classification Report
	
	![Combination (Over and Under) Sampling](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/Combination.png)

	- The balanced accuracy for the Undersampling model is 62.56%, which is slightly higher than the Undersampling model. The precision matches the other models. However, the recall number is higher for the "high_risk" classification than the previous models but the lower for the "low_risk" classification.
	
- Balanced Random Forest Classifier
	- Balanced Random Forest Classifier Imbalanced Classification Report
	
	![Balanced Random Forest Classifier](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/Balanced.png)

	- The balanced accuracy for the Balanced Random Forest model is 73.93% which is the second highest amongst all 6 models.  The precision for the "high_risk" classification is one point higher that the previous 4 models. The recall for the "low_risk" classification is much higher than the previous 4 models.
	
- Easy Ensemble AdaBoost Classifier
	- Easy Ensemble AdaBoost Classifier Imbalanced Classification Report
	
	![Easy Ensemble AdaBoost Classifier](https://github.com/jediracer/Credit_Risk_Analysis/blob/main/images/Easy_Ensemble.png)

	- The balanced accuracy for the Easy Ensemble AdaBoost model is 91.74% which is the highest of all 6 models. The precision and recall number are also the highest of all of the models.  Though, the precision number is still very low for the "high_risk" classification.

## Summary

- The best model of the 6 tested is the Easy Ensemble AdaBoost based on the accuracy, precision, recall and f1 scores.
- I would not recommend any of these models to determine if a loan is high risk or not.  The best precision score was only 6%. 