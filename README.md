## Credit Risk Analysis

### Overview of the analysis: 

The assignment this week is to use Supervised Machine Learning to predict credit card risk. We employed several different algorithms on a credit card credit dataset from Lending Club to determine the level of risk. We had to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. With the SMOTEENN algorithm we used a combinatorial approach of over and undersampling. Comparing two ML models (BalancedRandomForestClassifier and EasyEnsembleClassifier) was used to reduce bias and predict credit risk.



### Results: 

- Starting with Random Oversampling, we see that this model has a low balanced accuracy score of .59. Precision .90 and recall .69 scores are also high. 

<img width="752" alt="Screen Shot 2022-10-27 at 1 50 46 PM" src="https://user-images.githubusercontent.com/108151049/198362673-dc1d586f-b2c9-4aeb-a077-4ef8f98e508d.png">

- Using SMOTE Oversamling, we see that a slighly higher balanced accuracy score of .64 but that still isn't reassuring. And Undersampling provided similar results. They both have a precision score of .99. However Oversampling has a higher recall score of .74 compared to the undersampling model's recall score of .55. 

<img width="846" alt="Screen Shot 2022-10-27 at 2 06 22 PM" src="https://user-images.githubusercontent.com/108151049/198365652-8057c819-c472-414e-81e3-2cbec83bfb3c.png">
<img width="648" alt="Screen Shot 2022-10-27 at 2 08 52 PM" src="https://user-images.githubusercontent.com/108151049/198366120-e0b49031-7d8d-4e73-a4e2-42441b67bdf2.png">

- The SMOTEENN algorithm also didn't provide a high accuracy score but has a recall score of .62.

<img width="615" alt="Screen Shot 2022-10-27 at 2 09 55 PM" src="https://user-images.githubusercontent.com/108151049/198366289-bf220b17-5064-411b-bd45-790576b47916.png">

The two ML models (BalancedRandomForestClassifier and EasyEnsembleClassifier) have the highest balanced accuracy scores out of all the models with EasyEnsembleClassifier reporting back a .84. They also have high recall and precision scores.

<img width="623" alt="Screen Shot 2022-10-27 at 2 12 13 PM" src="https://user-images.githubusercontent.com/108151049/198366700-69c2616b-c7ba-4c9d-8ca1-d7b034f2c0b9.png">
<img width="610" alt="Screen Shot 2022-10-27 at 2 12 56 PM" src="https://user-images.githubusercontent.com/108151049/198366842-40f76a06-4097-4704-baf1-40c543ffefea.png">


### Summary: 

Out of all the models, Easy Ensemble Classifier had the highest balanced accuracy score, however, a .84 still isn't reassuring and fails to perform. Although .84 is the highest that still means .16 is missing. 

