# Credit_Risk_Analysis

The purpose of this analysis was to create a supervised machine learning model that could accurately predict credit risk from data patterns. 

Machine learning is the use of statistical algorithms to perform tasks such as learning from data patterns and making predictions. There are many different models—a model is a mathematical representation of something that happens in the real world.

In supervised learning, a model is initiated, or a template for the algorithm is created. Then it will analyze the data and attempt to learn patterns, which is also called fitting and training. After the data has been fit and trained, it will then make predictions.  

- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- The SMOTEEN algorithm which uses a combinatorial approach of over and undersampling data. 
- Then compare two machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier.

# Resources
- Software: Python, Anaconda and Jupyter Notebook
- Data Source: LoanStats_2019Q1.csv

# Goal: Building up my skills in data preparation, statistical reasoning, and machine learning. SMOTEEN Algorithm


# Results

### Deliverable 1: Use Resampling Models to Predict Credit Risk

- RandomOverSampler Model 


![oversampling_analysis](https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/oversampling.png)

The balanced accuracy score is 65%.

The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.

Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

- SMOTE Model

![SMOTE_Analysis](https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/SMOTE.png)

The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.


- ClusterCentroids Model

![cluster_analysis](https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/cluster.png)

Here the balanced accuracy score is down to about 52%.
The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%.

### Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk

- SMOTEENN Model 

The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.

![combinational_analysis](https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/cominational.png)


### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

- Balanced Random Forest Classifying

The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

<img width="568" alt="random_forest" src="https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/random_forest.png">


- Easy Ensemble Classifying

Now, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.



<img width="565" alt="easy_ensemble" src="https://github.com/acegal1/Credit_Risk_Analysis/blob/main/Resources/easy_ensemble.png">



# Summary

Found that the best model to detect if a loan is high risk or not, which is basically which model let the least amount of high risk loans pass through undetected would be to use the Easy Ensemble Classifying model.  The Easy Ensemble Classifying model was able to predict high risk loans.

