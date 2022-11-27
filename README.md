# Trajectory Consolidation using Supervised Clustering Algorithms
## Problem Statement 
Aerial Vehicles follow a guided approach based on Latitude, Longitude and Altitude. This information can be used for calculating the status of maneuvering for the aerial vehicles along the line of trajectory. This is a binary classification problem and Machine Learning can be leveraged for solving such problem. In this a methodology for deriving maneuvering status and its prediction using Linear, Distance Metric, Discriminant Analysis and Boosting Ensemble supervised learning methods are mentioned. Provided various metrics along the line in the results section that give condensed comparison of the appropriate algorithm for prediction of the maneuvering status. Also used LSTM to find the cluster of predicted part.

## Citation:

```
@article{gupta2022prediction,
  title={Prediction of Maneuvering Status for Aerial Vehicles using Supervised Learning Methods},
  author={Gupta, Abhishek and Thustu, Sarvesh and Thakor, Riti and Patil, Saniya and Joshi, Raunak and Laban, Ronald Melvin},
  journal={arXiv preprint arXiv:2206.10303},
  year={2022}
}

```

## Technology Stack
1. Python Packages for Data Processing and Cleaning
* Pandas
* Numpy

2. Deeplearning Framework
* PyTorch

## Results


* Precision 

This is a type of metric that defines the number of positive classes predicted from total number of positive classes. The foundation of the precision starts from Confusion Matrix. The elements of confusion matrix are True Positives, True Negatives, False Positives and False Negatives. 


o Table 1: Macro and Weighted Averaging Precision


| Algorithm | Macro | Weighted |
| :---         |     :---:      |          ---: |
| Logistic Regression |85% | 83% |
| KNN | 81% | 85% |
| LDA | 82% | 85% |
| CatBoost | 85% | 88% |


o Recall 

This is a metric that focuses on the positive predictions out of all the predictions. Recall also works considering the elements of confusion matrix.


o Table 2: Macro and Weighted Averaging Recall


|Algorithm | Macro | Weighted |
| :---         |     :---:      |          ---: |
|Logistic Regression | 66% | 82% |
|KNN | 79% | 85% |
| LDA | 78% | 86% |
| CatBoost | 81% | 88% |


* F1 - Score

The F1-Score is a metric of accuracy that is calculated using Precision and Recall. The metric clearly gives
assumption of the performance of the learning models.


o Table 3: F1-Score


|Algorithm | Score |
| :---         |     :---:      |
|Logistic Regression | 82% |
|KNN | 85% |
|LDA | 86% |
| CatBoost | 88% |


o Receiver Operating Characteristics and Area Under Curve


Receiver Operating Characteristics abbreviated as RoC is performance measurement metric for classification models considering thresholds. It is formed using True Positive Rate and False Positive Rate. But the RoC is not sufficient, Area Under Curve abbreviated as AUC is essential for representing the measure of separability. The value of AUC is plot between 0 and 1. Closer the AUC to 1, better is the algorithm.


![alt text](Results/roc-auc.png)

                                                         Figure 2: RoC Curve with AuC





























